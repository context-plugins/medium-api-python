
# List Response

## Structure

`ListResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `author` | `str` | Optional | `user_id` of the author |
| `claps` | `int` | Optional | - |
| `count` | `int` | Optional | Number of articles in the list |
| `created_at` | `str` | Optional | - |
| `description` | `str` | Optional | - |
| `id` | `str` | Optional | - |
| `last_item_inserted_at` | `str` | Optional | - |
| `name` | `str` | Optional | - |
| `responses_count` | `int` | Optional | - |
| `thumbnail` | `str` | Optional | Image URL |
| `voters` | `int` | Optional | - |

## Example

```python
from mediumapi.models.list_response import ListResponse

list_response = ListResponse(
    author='1985b61817c3',
    claps=48,
    count=18,
    created_at='2023-03-12 06:46:46',
    description='Collections of all the articles and resources related to Medium API',
    id='38f9e0f9bea6',
    last_item_inserted_at='2023-03-12 06:53:02',
    name='Medium API',
    responses_count=1,
    thumbnail='https://miro.medium.com/0*8f634a2860234802375db89fbfcccb5cc717f3fd.jpeg',
    voters=1
)
```

