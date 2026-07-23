
# User Lists Response

## Structure

`UserListsResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `lists` | `List[str]` | Optional | - |
| `user_id` | `str` | Optional | - |

## Example

```python
from mediumapi.models.user_lists_response import UserListsResponse

user_lists_response = UserListsResponse(
    lists=[
        'lists6'
    ],
    user_id='5142451174a3'
)
```

