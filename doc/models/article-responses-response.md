
# Article Responses Response

## Structure

`ArticleResponsesResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `str` | Optional | - |
| `responses` | `List[str]` | Optional | - |

## Example

```python
from mediumapi.models.article_responses_response import ArticleResponsesResponse

article_responses_response = ArticleResponsesResponse(
    id='67fa62fc1971',
    responses=[
        'responses3',
        'responses2',
        'responses1'
    ]
)
```

