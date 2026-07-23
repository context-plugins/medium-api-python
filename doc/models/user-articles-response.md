
# User Articles Response

## Structure

`UserArticlesResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `associated_articles` | `List[str]` | Optional | - |

## Example

```python
from mediumapi.models.user_articles_response import UserArticlesResponse

user_articles_response = UserArticlesResponse(
    associated_articles=[
        'associated_articles1',
        'associated_articles2',
        'associated_articles3'
    ]
)
```

