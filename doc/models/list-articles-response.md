
# List Articles Response

## Structure

`ListArticlesResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `str` | Optional | - |
| `list_articles` | `List[str]` | Optional | - |

## Example

```python
from mediumapi.models.list_articles_response import ListArticlesResponse

list_articles_response = ListArticlesResponse(
    id='38f9e0f9bea6',
    list_articles=[
        'list_articles9'
    ]
)
```

