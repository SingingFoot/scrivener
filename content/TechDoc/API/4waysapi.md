+++
title = "Four ways to make an API call in JS"
description = "This is an area for technical documentation"
weight = 1
+++

There are many ways to make an API call in different programming languages. In JavaScript an API could be called in four ways: 

- XMLHttpRequest
- Fetch API
- Axios
- JQuery

Use JSON [Placeholder](https://jsonplaceholder.typicode.com/users) service to get API data. It has an endpoint with 10 users data.


## How to present API data in a table

If you need to present API in the table, create an index.html file with the code showed below.

{{< collapse title="index.html to present API data in a table" >}} 
{{< code lang="html" >}} 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css">
</head>
<body>
    <h1 class="text-center">Storing API request in table</h1>
    <div class="container">
        <table class="table table-bordered">
            <thead>
              <tr class="table-primary">
                <th scope="col">Id</th>
                <th scope="col">Name</th>
                <th scope="col">Username</th>
                <th scope="col">Email</th>
                <th scope="col">Address</th>
              </tr>
            </thead>
            <tbody id="table_body">
              <tr>
                <td>name</td>
                <td>Mark</td>
                <td>Otto</td>
                <td>@mdo</td>
                <td>@mdo</td>
              </tr>
            </tbody>
          </table>
    </div>
<script src="script.js"></script>
</body>
</html> 
{{< /code >}}
{{< /collapse >}}


## XMLHttpRequest

All modern browsers have a built-in XMLHttpRequest object to request data from a server. The XMLHttpRequest object can be used to request data from a web server. One can see in the example below that API data could be presented in two ways:
1. As a constant const `responseAPI` to get all the data in the table.
2. In the browser console `console.log(responseAPI)`

{{< collapse title="XMLHttpRequest gets API data in such a way" >}} 
{{< code lang="html" >}} 

const request = new XMLHttpRequest();
request.open("GET", "https://jsonplaceholder.typicode.com/users");
request.send();//to get API data in Network => Preview browser tab
request.onload = ()=>{
    console.log(request);
    if(request.status === 200) {
        const responseAPI = JSON.parse(request.response);// to get API data as JSON in responseAPI constant
        console.log(responseAPI); // to get API data as JSON in browser Console
        let tableData="";
        responseAPI.map((values)=>{
        tableData+=`<tr>
        <td>${values.id}</td>
        <td>${values.name}</td>
        <td>${values.username}</td>
        <td>${values.email}</td>
        <td>${values.address.street}, ${values.address.suite}, ${values.address.city}, ${values.address.zipcode},</td>
      </tr>`;
    });
    document.getElementById("table_body").innerHTML=tableData;
    } else {
        console.log(`error ${request.status}`) // to handle errors
    }
}
{{< /code >}} 
{{< /collapse >}} 

## Fetch API

The Fetch API provides an interface for fetching resources (including across the network). It will seem familiar to anyone who has used `XMLHttpRequest`, but the new API provides a more powerful and flexible feature set.
The `fetch()` method takes one mandatory argument, the path to the resource you want to fetch. It returns a Promise that resolves to the Response to that request — as soon as the server responds with headers — even if the server response is an HTTP error status. 
The API data received from the server is stored into `json` object and can be placed in a constant

{{< collapse title="In the example below API data placed in responseAPI constant and presented in a table" >}} 
{{< code lang="html" >}} 

fetch('https://jsonplaceholder.typicode.com/users')
    .then(response=>{
        return response.json();
    }).then(json=>{
        console.log(json);
        const responseAPI = json;
        let tableData="";
        responseAPI.map((values)=>{
        tableData+=`<tr>
        <td>${values.id}</td>
        <td>${values.name}</td>
        <td>${values.username}</td>
        <td>${values.email}</td>
        <td>${values.address.street}, ${values.address.suite}, ${values.address.city}, ${values.address.zipcode},</td>
      </tr>`;
    });
    document.getElementById("table_body").innerHTML=tableData;
    })
{{< /code >}} 
{{< /collapse >}} 

<br><br>

There is also a second approach with fetch API using async function

{{< collapse title="fetch API using async function" >}} 
{{< code lang="html" >}} 
async function getUsers(){
    let response = await fetch('https://jsonplaceholder.typicode.com/users');
    let data = await response.json();
    return data;
}

getUsers().then(response=>{
    console.log(response);
    const responseAPI = response;
    let tableData="";
    responseAPI.map((values)=>{
    tableData+=`<tr>
    <td>${values.id}</td>
    <td>${values.name}</td>
    <td>${values.username}</td>
    <td>${values.email}</td>
    <td>${values.address.street}, ${values.address.suite}, ${values.address.city}, ${values.address.zipcode},</td>
  </tr>`;
});
document.getElementById("table_body").innerHTML=tableData;
})
{{< /code >}} 
{{< /collapse >}} 

## Axios

Axios is a promise-based HTTP Client for node.js and the browser. It is isomorphic (= it can run in the browser and nodejs with the same codebase). On the server-side it uses the native node.js http module, while on the client (browser) it uses XMLHttpRequests.

To use the client visit its [Axios website](https://axios-http.com/docs/intro) to find the corresponding CDN. Copy and paste that CDN to your index.html file

{{< code lang="html" >}}    
<script src="https://cdn.jsdelivr.net/npm/axios/dist/axios.min.js"></script>
{{< /code >}}

{{< collapse title="Use Axios like this to present API data in a table" >}} 
{{< code lang="html" >}} 

axios.get('https://jsonplaceholder.typicode.com/users')
     .then(response=>{
        console.log(response.data);
    const responseAPI = response.data;
    let tableData="";
    responseAPI.map((values)=>{
    tableData+=`<tr>
    <td>${values.id}</td>
    <td>${values.name}</td>
    <td>${values.username}</td>
    <td>${values.email}</td>
    <td>${values.address.street}, ${values.address.suite}, ${values.address.city}, ${values.address.zipcode},</td>
  </tr>`;
});
document.getElementById("table_body").innerHTML=tableData;
     }, err=>{
        console.log(err);
     })
{{< /code >}} 
{{< /collapse >}} 


## JQuery

jQuery is a fast, small, and feature-rich JavaScript library. It makes things like HTML document traversal and manipulation, event handling, animation, and Ajax much simpler with an easy-to-use API that works across a multitude of browsers. 

To use the jQuery visit the [CDNJS Library](https://cdnjs.com/libraries/jquery) to find the corresponding CDN. Copy and paste that CDN to your index.html file

{{< code lang="html">}} 
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.1/jquery.min.js"></script>
{{< /code >}} 

{{< collapse title="Use jQuery like this to present API data in a table" >}} 
{{< code lang="html" >}} 

$(document).ready(function(){
    $.ajax({
        url:'https://jsonplaceholder.typicode.com/users',
        type:"GET",
        success:function(result){
            console.log(result)
            const responseAPI = result;
            let tableData="";
            responseAPI.map((values)=>{
            tableData+=`<tr>
            <td>${values.id}</td>
            <td>${values.name}</td>
            <td>${values.username}</td>
            <td>${values.email}</td>
            <td>${values.address.street}, ${values.address.suite}, ${values.address.city}, ${values.address.zipcode},</td>
            </tr>`;
            });
            document.getElementById("table_body").innerHTML=tableData;
        },
        error:function(err){
            console.log(err);
        }

    })
})
{{< /code >}} 
{{< /collapse >}} 



