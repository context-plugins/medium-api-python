
# Search Users Response

## Structure

`SearchUsersResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `search_query` | `str` | Optional | - |
| `users` | `List[str]` | Optional | - |

## Example

```python
from mediumapi.models.search_users_response import SearchUsersResponse

search_users_response = SearchUsersResponse(
    search_query='data engineer',
    users=[
        'users1'
    ]
)
```

