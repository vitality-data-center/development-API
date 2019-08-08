# **Data Access API**
----
  This API provides the access to the datasets and their metadata stored at the backend. Each user should log in and use his account to browse the datasets available in the data center. 


* **Method:**
  
  <_The request type: `POST`_>

## **Request parameters**

| Parameter | Description                                                                                 |
|:-------------------|:--------------------------------------------------------------------------------------------|
| `user_id`   | user id |
| `key_words`  | this is optional and still needs further discussions. Ideally the key works are from users, and is a string with a set of words should be separated by commas, such as {survey} | 
   



 ## **Response:**
The following elements may be present in the response, and will be visualized in the [frontend](https://vitality-data-center.github.io/) 
 
| Value | Description                                                                                 |
|:-------------------|:--------------------------------------------------------------------------------------------|
| `id`   | the ID of the dataset. |
| `own_id`   | the ID of the owner of the dataset. |
| `title`   | title of the dataset. |
| `time_c`  | the time when the dataset was created. | 
| `time_u`  | the time when the dataset was uploaded. | 
| `size`  | size of the dataset.                |
| `means` | the means that was used for collection of the dataset|
| `permission` | access permission, possible values: 0=closed; 1=need permission from the owner; 2=open|
| `context` | the context related to the dataset, possible values: 0=behavioral data; 1=environmental data; 2=unknown|
| `description` | a short description of the dataset|


