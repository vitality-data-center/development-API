**Data Access API**
----
  This API provides the access to the datasets and their metadata stored at the backend.

* **URL**

  <_The URL Structure (path only, no root url)_>

* **Method:**
  
  <_The request type_>

  `GET` | `POST` | `DELETE` | `PUT`

## **Request parameters**
| Parameter | Description                                                                                 |
|:-------------------|:--------------------------------------------------------------------------------------------|
| `title`    | Title of the dataset. |
| 'size' | Size of the dataset.                |
| `--log <log_file>` | Log console output to a file.                                                               |


 


 ## **Response:**

  <_Most endpoints will have many ways they can fail. From unauthorized access, to wrongful parameters etc. All of those should be liste d here. It might seem repetitive, but it helps prevent assumptions from being made where they should be._>

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `{ error : "Log in" }`


