+++
title = "API terms"
description = "This is an area for technical documentation"
weight = 4
+++

## Resource URL

`https://api.openweathermap.org/surfreport/{beachId}`

## Endpoint 

`/surfreport/{beachId}`

## Path parameter

Path parameter should be represented in curly braces): `{beachId}`

## Parameters

Parameters are options you can pass with the endpoint (such as specifying the response format or the amount returned) to influence the response. 
There are several types of parameters: 

- **header parameters:** are included in the request header, usually related to authorization. 
- **path parameters:** are within the path of the endpoint, before the query string (?). These are usually set off within curly braces. 
- **query string parameters:** in the query string of the endpoint, after the ?.

Regardless of the parameter type, define the following with each parameter:

- Data type
- Max and min value

These data types are the most common with REST APIs:

**string**: An alphanumeric sequence of letters and/or numbers

**integer**: A whole number — can be positive or negative

**boolean**: True or false value

**object**: Key-value pairs in JSON format

**array**: A list of values

In addition to specifying the data type, the parameters should indicate the maximum, minimum, and allowed values if appropriate.

The method defines the operation with the resource. Briefly, each method is as follows:

{{< button style="success" >}} GET {{< /button >}} Retrieves a resource

{{< button style="info" >}} POST {{< /button >}} Creates a resource

{{< button style="secondary" >}} PUT {{< /button >}} Updates or creates within an existing resource

{{< button style="primary" >}} PATCH {{< /button >}} Partially modifies an existing resource

{{< button style="danger" >}} DELETE {{< /button >}} Removes the resource

## Request bodies

Request bodies are closely similar to parameters but are not technically a parameter. In OpenAPI v2.0, request bodies were classified as a type of parameter, but in v3.0, they are not considered a parameter but rather a path property.

```
{
"days": 2,
"units": "imperial",
"time": 1433524597
}
```