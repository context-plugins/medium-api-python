
# Publication Id for Response

## Structure

`PublicationIdForResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `publication_id` | `str` | Optional | Unique hash id of the publication. |
| `publication_slug` | `str` | Optional | Same publication slug that you passed in the path parameters. |

## Example

```python
from mediumapi.models.publication_id_for_response import PublicationIdForResponse

publication_id_for_response = PublicationIdForResponse(
    publication_id='29038077e4c6',
    publication_slug='codex'
)
```

