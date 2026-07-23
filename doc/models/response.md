
# Response

## Structure

`Response`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `developer` | `str` | Optional | Full name of the API's developer |
| `documentation` | `str` | Optional | Link to the Medium API's documentation |
| `email` | `str` | Optional | Email ID of the developer |
| `linkedin` | `str` | Optional | LinkedIn Page URL |
| `name` | `str` | Optional | Full name of the API |
| `twitter` | `str` | Optional | Twitter Profile URL |
| `website` | `str` | Optional | Link to the Medium API's website |

## Example

```python
from mediumapi.models.response import Response

response = Response(
    developer='Nishu Jain',
    documentation='https://docs.mediumapi.com',
    email='nishu@mediumapi.com',
    linkedin='https://www.linkedin.com/company/medium-api',
    name='Medium API',
    twitter='https://twitter.com/medium_api',
    website='https://mediumapi.com'
)
```

