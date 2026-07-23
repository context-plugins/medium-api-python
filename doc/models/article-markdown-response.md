
# Article Markdown Response

## Structure

`ArticleMarkdownResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `markdown` | `str` | Optional | - |

## Example

```python
from mediumapi.models.article_markdown_response import ArticleMarkdownResponse

article_markdown_response = ArticleMarkdownResponse(
    markdown='# Article title\n## Article Subtitle\nArticle **Content** with lot of _markups_ ....\n![Images Alt](Image URL)\n'
)
```

