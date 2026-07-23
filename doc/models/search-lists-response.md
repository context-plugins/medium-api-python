
# Search Lists Response

## Structure

`SearchListsResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `lists` | `List[str]` | Optional | - |
| `search_query` | `str` | Optional | - |

## Example

```python
from mediumapi.models.search_lists_response import SearchListsResponse

search_lists_response = SearchListsResponse(
    lists=[
        'lists0',
        'lists1',
        'lists2'
    ],
    search_query='artificial intelligence'
)
```

