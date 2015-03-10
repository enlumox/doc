Error responses
---------------

When an error occurs the error field in a response is present.

```
{"result":null,"error":{"code":1502,"message":"field name is required"}}
```
Whenever a non functional error occurs there is also a reference field in the error payload. The reference field contains a uuid which has been logged in the backend. Use this uuid as reference to the issue in the support ticket.

Technical
---------

| Code |Description |
|------|:------------|
| 1000 | An error occured with the datastore service |
| 1001 | An error occured with the datastore database |
| 1002 | An error occured parsing json in the backend |


Functional
----------

| Code |Description |
|------|:-----------|
| 1500 | The requested entity was not found |
| 1501 | Invalid json |
| 1502 | The "name" field is missing in the json payload | 
