
# Related Tags Response

## Structure

`RelatedTagsResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `given_tag` | `str` | Optional | - |
| `related_tags` | `List[str]` | Optional | - |

## Example

```python
from mediumapi.models.related_tags_response import RelatedTagsResponse

related_tags_response = RelatedTagsResponse(
    given_tag='blockchain',
    related_tags=[
        'related_tags3'
    ]
)
```

