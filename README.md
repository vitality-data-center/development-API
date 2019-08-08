**Data Access API**
----
  This API provides the access to the datasets and their metadata stored at the backend.

* **URL**

  <_The URL Structure (path only, no root url)_>

* **Method:**
  
  <_The request type_>

  `GET` | `POST` | `DELETE` | `PUT`

## **Request parameters**




 


 ## **Response:**
The following elements may be present in the response, and will be visualized in the [frontend](https://vitality-data-center.github.io/) 
 
 
| Parameter | Description                                                                                 |
|:-------------------|:--------------------------------------------------------------------------------------------|
| `title`   | title of the dataset. |
| `time_c`  | the time when the dataset was created. | 
| `time_u`  | the time when the dataset was uploaded. | 
| `size`  | size of the dataset.                |
| `means` | the means that was used for collection of the dataset|
| `permission` | access permission, possible values: 0=closed; 1=need permission from the owner; 2=open|
| `context` | the context related to the dataset, possible values: 0=behavioral data; 1=environmental data; 2=unknown|
| `description` | a short description of the dataset|


