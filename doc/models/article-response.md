
# Article Response

## Structure

`ArticleResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `author` | `str` | Optional | - |
| `claps` | `int` | Optional | - |
| `id` | `str` | Optional | - |
| `image_url` | `str` | Optional | - |
| `is_locked` | `bool` | Optional | - |
| `is_series` | `bool` | Optional | - |
| `lang` | `str` | Optional | - |
| `last_modified_at` | `str` | Optional | - |
| `publication_id` | `str` | Optional | - |
| `published_at` | `str` | Optional | - |
| `reading_time` | `float` | Optional | - |
| `responses_count` | `int` | Optional | - |
| `subtitle` | `str` | Optional | - |
| `tags` | `List[str]` | Optional | - |
| `title` | `str` | Optional | - |
| `topics` | `List[str]` | Optional | - |
| `url` | `str` | Optional | - |
| `voters` | `int` | Optional | - |
| `word_count` | `int` | Optional | - |

## Example

```python
from mediumapi.models.article_response import ArticleResponse

article_response = ArticleResponse(
    author='1985b61817c3',
    claps=53,
    id='f06086080568',
    image_url='https://miro.medium.com/1*W0wM9xIeeIR3_Oo0E_thaA.png',
    is_locked=True,
    is_series=False,
    lang='en',
    last_modified_at='2021-05-28 04:22:48',
    publication_id='e7040e67514c',
    published_at='2020-08-25 11:08:18',
    reading_time=3.5720125786164,
    responses_count=10,
    subtitle='Re-energize your relationship in the midst of a crisis',
    title='4 Tips to Strengthen Your Bonds — Now',
    url='https://medium.com/age-of-awareness/re-energizing-your-relationship-in-the-midst-of-a-crisis-f06086080568',
    voters=3,
    word_count=845
)
```

