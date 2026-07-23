
# Search Articles Response

## Structure

`SearchArticlesResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `articles` | `List[str]` | Optional | - |
| `search_query` | `str` | Optional | - |

## Example

```python
from mediumapi.models.search_articles_response import SearchArticlesResponse

search_articles_response = SearchArticlesResponse(
    articles=[
        'articles7',
        'articles6'
    ],
    search_query='startup'
)
```

