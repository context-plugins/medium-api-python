
# User Top Articles Response

## Structure

`UserTopArticlesResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `associated_articles` | `List[str]` | Optional | - |

## Example

```python
from mediumapi.models.user_top_articles_response import UserTopArticlesResponse

user_top_articles_response = UserTopArticlesResponse(
    associated_articles=[
        'associated_articles5',
        'associated_articles6'
    ]
)
```

