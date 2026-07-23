
# Search Tags Response

## Structure

`SearchTagsResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `search_query` | `str` | Optional | - |
| `tags` | `List[str]` | Optional | - |

## Example

```python
from mediumapi.models.search_tags_response import SearchTagsResponse

search_tags_response = SearchTagsResponse(
    search_query='blockchain',
    tags=[
        'tags3'
    ]
)
```

