Errors
======

Error responses
---------------

When an error occurs the error field in a response is present.

```
{"result":null,"error":{"code":1501,"message":"field name is required"}}
```
Whenever a non functional error occurs there is also a reference field in the error payload. The reference field contains a uuid which has been logged in the backend. Use this uuid as reference to the issue in the support ticket.

Technical
---------

| Code | Description |
|------|-------------|
| 1001 | An error occured with the datastore backend |
| 1002 | An error occured parsing json in the backend |

Functional
----------

| Code | Description |
|------|------------|
| 1500 | The requested entity was not found |
| 1501 | The "name" field is missing in the json payload | 
