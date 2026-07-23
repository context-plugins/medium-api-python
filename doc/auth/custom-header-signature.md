
# Custom Header Signature



Documentation for accessing and setting credentials for ApiHost.

## Auth Credentials

| Name | Type | Description | Getter |
|  --- | --- | --- | --- |
| x-rapidapi-host | `str` | - | `x_rapidapi_host` |



**Note:** Auth credentials can be set using `ApiHostCredentials` object, passed in as named parameter `api_host_credentials` in the client initialization.

## Usage Example

### Client Initialization

You must provide credentials in the client as shown in the following code snippet.

```python
from mediumapi.http.auth.api_host import ApiHostCredentials
from mediumapi.mediumapi_client import MediumapiClient

client = MediumapiClient(
    api_host_credentials=ApiHostCredentials(
        x_rapidapi_host='x-rapidapi-host'
    )
)
```


