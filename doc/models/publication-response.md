
# Publication Response

## Structure

`PublicationResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `creator` | `str` | Optional | - |
| `description` | `str` | Optional | - |
| `editors` | `List[str]` | Optional | - |
| `facebook_pagename` | `str` | Optional | - |
| `followers` | `int` | Optional | - |
| `id` | `str` | Optional | - |
| `instagram_username` | `str` | Optional | - |
| `name` | `str` | Optional | - |
| `slug` | `str` | Optional | - |
| `tagline` | `str` | Optional | - |
| `tags` | `List[str]` | Optional | - |
| `twitter_username` | `str` | Optional | - |
| `url` | `str` | Optional | - |

## Example

```python
from mediumapi.models.publication_response import PublicationResponse

publication_response = PublicationResponse(
    creator='8a819983d566',
    description='Towards AI is the world\'s leading AI and technology publication. Publishing unbiased AI and technology-related articles. Read by thought-leaders and decision-makers around the world.',
    editors=[
        'editors1',
        'editors2',
        'editors3'
    ],
    facebook_pagename='towardsAl',
    followers=25260,
    id='98111c9905da',
    instagram_username='towards_ai',
    name='Towards AI',
    slug='towards-artificial-intelligence',
    tagline='The World\'s Leading AI and Technology Publication',
    twitter_username='towards_AI',
    url='pub.towardsai.net'
)
```

