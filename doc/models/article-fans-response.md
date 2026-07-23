
# Article Fans Response

## Structure

`ArticleFansResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `article_id` | `str` | Optional | - |
| `count` | `int` | Optional | - |
| `voters` | `List[str]` | Optional | - |

## Example

```python
from mediumapi.models.article_fans_response import ArticleFansResponse

article_fans_response = ArticleFansResponse(
    article_id='67fa62fc1971',
    count=145,
    voters=[
        'voters8',
        'voters9'
    ]
)
```

