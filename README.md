# **Data Access API**
----
  This API provides the access to the datasets and their metadata stored at the backend. Every user should log in and uses his/her account to browse and access the datasets available in the data center. 


* **Method:**
  
  <_The request type: `POST`_>

## **Request parameters**

| Parameter | Description                                                                                 |
|:-------------------|:--------------------------------------------------------------------------------------------|
| `user_id`   | user id |
| `key_words`  | this is optional and still needs further discussions. Ideally the key works should from users, and is a string with a set of words that separated by commas, such as {noise, running} | 
   



 ## **Response:**
The response results may contain information of multiple datasets, so the response may be formatted into a [json array](https://stackoverflow.com/questions/12289844/difference-between-jsonobject-and-jsonarray), and each element in this array corresponds to a json object, which refers to a dataset. The following elements may be present in the response, and will be visualized in the [frontend](https://vitality-data-center.github.io/) 
 
| Value | Description                                                                                 |
|:-------------------|:--------------------------------------------------------------------------------------------|
| `id`   | the ID of the dataset. |
| `owner_id`   | the ID of the owner of the dataset. |
| `title`   | title of the dataset. |
| `time_c`  | the time when the dataset was created. | 
| `time_u`  | the time when the dataset was uploaded. | 
| `size`  | size of the dataset.                |
| `means` | the means that was used for collection of the dataset|
| `permission` | access permission, possible values: 0=closed; 1=need permission from the owner; 2=open|
| `context` | the context related to the dataset, possible values: 0=behavioral data; 1=environmental data; 2=unknown|
| `description` | a short description of the dataset|
| `link` | the link access to the dataset (still needs to be decided)|


