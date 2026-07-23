
# Custom Header Signature



Documentation for accessing and setting credentials for ApiKey.

## Auth Credentials

| Name | Type | Description | Getter |
|  --- | --- | --- | --- |
| x-rapidapi-key | `str` | - | `x_rapidapi_key` |



**Note:** Auth credentials can be set using `ApiKeyCredentials` object, passed in as named parameter `api_key_credentials` in the client initialization.

## Usage Example

### Client Initialization

You must provide credentials in the client as shown in the following code snippet.

```python
from mediumapi.http.auth.api_key import ApiKeyCredentials
from mediumapi.mediumapi_client import MediumapiClient

client = MediumapiClient(
    api_key_credentials=ApiKeyCredentials(
        x_rapidapi_key='x-rapidapi-key'
    )
)
```


