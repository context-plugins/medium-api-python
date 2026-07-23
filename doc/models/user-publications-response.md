
# User Publications Response

## Structure

`UserPublicationsResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `publications` | `List[str]` | Optional | - |
| `user_id` | `str` | Optional | - |

## Example

```python
from mediumapi.models.user_publications_response import UserPublicationsResponse

user_publications_response = UserPublicationsResponse(
    publications=[
        'publications0',
        'publications9',
        'publications8'
    ],
    user_id='14d5c41e0264'
)
```

