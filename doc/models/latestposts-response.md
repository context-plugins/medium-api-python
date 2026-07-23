
# Latestposts Response

## Structure

`LatestpostsResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `latestposts` | `List[str]` | Optional | - |

## Example

```python
from mediumapi.models.latestposts_response import LatestpostsResponse

latestposts_response = LatestpostsResponse(
    latestposts=[
        'latestposts4',
        'latestposts3',
        'latestposts2'
    ]
)
```

