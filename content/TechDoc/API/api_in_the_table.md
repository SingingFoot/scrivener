---
sidebar_position: 2
displayed_sidebar: techdoc
---

# How to place API in a table


## Create some boiler plates

To present API data in a table online create three files in a folder:

    index.html
    script.js
    style.css

Then add bootstrap code to index.html to get the table fast. Open the [Bootstrap](https://getbootstrap.com/) service, click on the "Read the Docs" button and find CDN links paragraph on the page. 
<details>
  <summary>Copy the link and add it to index.html</summary>

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>API data in table</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css">
</head>
<body>
    
</body>
</html>
```
</details>

## Find a free API online

Open the [FakeStoreApi](https://fakestoreapi.com/docs) service. FakeStoreApi is a free online REST API that you can use whenever you need Pseudo-real data for your e-commerce or shopping website without running any server-side code. It's awesome for teaching purposes, sample codes, tests, etc.

You can find all the API data by clicking the [Products](https://fakestoreapi.com/products) link. 

## Add HTML tags

Add the title to your website with H1 tag. Find the [Tables](https://getbootstrap.com/docs/5.2/content/tables/#overview) paragraph in the Bootstrap website and copy the code into your index.html file under the H1 tag. Place the table code inside the "container" div. 
You also can add class="table-primary" to the first table's row (inside `<tr>` tag) to make in light blue. To add borders to the table add class="table table-bordered" to the `<table>` tag.
Change titles into the table's header according to the API (Title, Description, Price and Image).

<details>
  <summary>The result should look like this.</summary>

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>API data in table</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css">
</head>
<body>
    <h1 class="text-center">Storing API data in table</h1>
    <div class="container">
        <table class="table table-bordered">
            <thead>
              <tr class="table-primary">
                <th scope="col">#</th>
                <th scope="col">First</th>
                <th scope="col">Last</th>
                <th scope="col">Handle</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <th scope="row">1</th>
                <td>Mark</td>
                <td>Otto</td>
                <td>@mdo</td>
              </tr>
              <tr>
                <td>2</td>
                <td>Jacob</td>
                <td>Thornton</td>
                <td>@fat</td>
              </tr>
              <tr>
                <th scope="row">3</th>
                <td colspan="2">Larry the Bird</td>
                <td>@twitter</td>
              </tr>
            </tbody>
          </table>
    </div>

</body>
</html>
```
</details>

Change the first cell in the first row from "1" to "name" and delete second and third rows. Add id to "tbody" tag: `<tbody id="table_body">`.

<details>
  <summary>The prepared index.html should look like this.</summary>

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>API data in table</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css">
</head>
<body>
    <h1 class="text-center">Storing API data in table</h1>
    <div class="container">
        <table class="table table-bordered">
            <thead>
              <tr class="table-primary">
                <th scope="col">Title</th>
                <th scope="col">Description</th>
                <th scope="col">Price</th>
                <th scope="col">Image</th>
              </tr>
            </thead>
            <tbody id="table_body">
              <tr>
                <td>name</td>
                <td>Mark</td>
                <td>Otto</td>
                <td>@mdo</td>
              </tr>
            </tbody>
          </table>
    </div>

</body>
</html>
```

</details>

## Add JS code to fetch data from API

Add `<script src="script.js"></script>` code before the `</body>` closing tag. Use promises with "fetch" function. Add the [Products](https://fakestoreapi.com/products) API link as a parameter. 

<details>
  <summary>Get the data and convert them from JSON to an object like this.</summary>

```
fetch("https://fakestoreapi.com/products").then((data)=>{
    // console.log(data); the data is in json format
    return data.json(); // the data is converted to an object
}).then((objectData)=>{
    //console.log(objectData); the data is presented as an object in your browser console
})
```
</details>

## Add the API data to the table

If you add the index "0" to the "objectData" parameter, only the first element of the object will be presented in the browser console.
<details>
  <summary>See the example.</summary>

```
fetch("https://fakestoreapi.com/products").then((data)=>{
    // console.log(data); the data is in json format
    return data.json(); // the data is converted to an object
}).then((objectData)=>{
    //console.log(objectData[0]); the data is presented as an object in your browser console, [0] index shows only the first element in the console 
})
```
</details>

Create empty "tableData" variable and use "map" method for "objectData" to present all the data from API.
<details>
  <summary>See the example with "map" method.</summary>

```
fetch("https://fakestoreapi.com/products").then((data)=>{
    // console.log(data); the data is in json format
    return data.json(); // the data is converted to an object
}).then((objectData)=>{
    console.log(objectData[0].title); //the data is presented as an object in your browser console
    let tableData="";
    objectData.map((values)=>{
        tableData=`<h1>${values.title}</h1>`;
    })
})
```
</details>

Add the id to "tbody" tag `<tbody id="table_body">` and use it in the "getElementById" method with "innerHTML" method.
<details>
  <summary>See the example with "getElementById" method with "innerHTML" method.</summary>

```
fetch("https://fakestoreapi.com/products").then((data)=>{
    // console.log(data); the data is in json format
    return data.json(); // the data is converted to an object
}).then((objectData)=>{
    console.log(objectData[0].title); //the data is presented as an object in your browser console
    let tableData="";
    objectData.map((values)=>{
        tableData=`<h1>${values.title}</h1>`;
    });
    document.getElementById("table_body").innerHTML=tableData;
})
```
</details>

But you can have only the last title (with "id":20) from the API in such a way. Add the "+" sign before the "=" sign in the line below to get all the data from the API.

```
tableData+=`<h1>${values.title}</h1>`;
``` 
Then change the `<h1>` tag with the entire table row from the index.html file in the "tableData" variable.
``` 
tableData+=`<tr>
        <td>name</td>
        <td>Mark</td>
        <td>Otto</td>
        <td>@mdo</td>
      </tr>`;
``` 
After that you need to replace the hardcoded values (name, Mark, Otto and @mdo) with the API values in the "tableData" variable. Pay attention that all the images must be placed into the `<img src>` tag.

```
tableData+=`<tr>
        <td>${values.title}</td>
        <td>${values.description}</td>
        <td>${values.price}</td>
        <td><img src="${values.image}"/></td>
      </tr>`;  
``` 

## Style the images

You can see that all the images are fetched in their original size, so they are too large. You can limit the images sizes in the style.css file. Link that file in your index.html file like this.
```
<link rel="stylesheet" href="style.css">
```
Then add the image size rule to the "style.css" file.
```
img{
    width: 100px;
}
```

## Handle errors with "catch" method

There could be errors, if API is unavailable. 
<details>
  <summary>To handle with it add "catch" method to the function.</summary>

```
fetch("https://fakestoreapi.com/products").then((data)=>{
    // console.log(data); the data is in json format
    return data.json(); // the data is converted to an object
}).then((objectData)=>{
    //console.log(objectData[0].title); //the data is presented as an object in your browser console
    let tableData="";
    objectData.map((values)=>{
        tableData+=`<tr>
        <td>${values.title}</td>
        <td>${values.description}</td>
        <td>${values.price}</td>
        <td><img src="${values.image}"/></td>
      </tr>`; 
    });
    document.getElementById("table_body").innerHTML=tableData;
}).catch((err)=>{
    console.log(err);
})
```
</details>


