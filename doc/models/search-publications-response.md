
# Search Publications Response

## Structure

`SearchPublicationsResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `publications` | `List[str]` | Optional | - |
| `search_query` | `str` | Optional | - |

## Example

```python
from mediumapi.models.search_publications_response import SearchPublicationsResponse

search_publications_response = SearchPublicationsResponse(
    publications=[
        'publications6'
    ],
    search_query='mental health'
)
```

