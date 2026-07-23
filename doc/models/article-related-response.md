
# Article Related Response

## Structure

`ArticleRelatedResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `str` | Optional | - |
| `related_articles` | `List[str]` | Optional | - |

## Example

```python
from mediumapi.models.article_related_response import ArticleRelatedResponse

article_related_response = ArticleRelatedResponse(
    id='67fa62fc1971',
    related_articles=[
        'related_articles3',
        'related_articles4'
    ]
)
```

