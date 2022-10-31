---
sidebar_position: 4
displayed_sidebar: techdoc
---

# API terms

Resource URL: https://api.openweathermap.org/surfreport/{beachId}

Endpoint: /surfreport/{beachId}

Path parameter (it should be represented in curly braces): {beachId}

Parameters are options you can pass with the endpoint (such as specifying the response format or the amount returned) to influence the response. 
There are several types of parameters: 

- **header parameters:** are included in the request header, usually related to authorization. 
- **path parameters:** are within the path of the endpoint, before the query string (?). These are usually set off within curly braces. 
- **query string parameters:** in the query string of the endpoint, after the ?.

Request bodies are closely similar to parameters but are not technically a parameter.

Regardless of the parameter type, define the following with each parameter:

- Data type
- Max and min value

The method defines the operation with the resource. Briefly, each method is as follows:

{{< button style="green" >}} GET {{< /button >}} Retrieves a resource
{{< button style="blue" >}} POST {{< /button >}} Creates a resource
{{< button style="violet" >}} PUT {{< /button >}} Updates or creates within an existing resource
{{< button style="orange" >}} PATCH {{< /button >}} Partially modifies an existing resource
{{< button style="red" >}} DELETE {{< /button >}} Removes the resource

