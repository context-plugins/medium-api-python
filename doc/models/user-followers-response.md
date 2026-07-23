
# User Followers Response

## Structure

`UserFollowersResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `followers` | `List[str]` | Optional | - |
| `id` | `str` | Optional | - |

## Example

```python
from mediumapi.models.user_followers_response import UserFollowersResponse

user_followers_response = UserFollowersResponse(
    followers=[
        'followers4'
    ],
    id='14d5c41e0264'
)
```

