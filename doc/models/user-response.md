
# User Response

## Structure

`UserResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `allow_notes` | `bool` | Optional | - |
| `bio` | `str` | Optional | - |
| `followers_count` | `int` | Optional | - |
| `following_count` | `int` | Optional | - |
| `fullname` | `str` | Optional | - |
| `has_list` | `bool` | Optional | - |
| `id` | `str` | Optional | - |
| `image_url` | `str` | Optional | - |
| `is_book_author` | `bool` | Optional | - |
| `is_suspended` | `bool` | Optional | - |
| `is_writer_program_enrolled` | `bool` | Optional | - |
| `medium_member_at` | `str` | Optional | - |
| `top_writer_in` | `List[str]` | Optional | - |
| `twitter_username` | `str` | Optional | - |
| `username` | `str` | Optional | - |

## Example

```python
from mediumapi.models.user_response import UserResponse

user_response = UserResponse(
    allow_notes=False,
    bio='Obsessed with Tech Biz Arts &amp; Words; Does NOT dumb down the writing; Skilled Wordsmith; Delivers the best',
    followers_count=450,
    following_count=4,
    fullname='Nishu Jain',
    has_list=True,
    id='1985b61817c3',
    image_url='https://miro.medium.com/1*C92Hx7k9nRM7TPlrmhgW9w.jpeg',
    is_book_author=False,
    is_suspended=False,
    medium_member_at='2020-06-24 16:05:46',
    twitter_username='one_anachronism',
    username='nishu-jain'
)
```

