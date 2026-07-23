
# User following Response

## Structure

`UserFollowingResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `following` | `List[str]` | Optional | - |
| `id` | `str` | Optional | - |

## Example

```python
from mediumapi.models.user_following_response import UserFollowingResponse

user_following_response = UserFollowingResponse(
    following=[
        'following3'
    ],
    id='14d5c41e0264'
)
```

