
# Publication Newsletter Response

## Structure

`PublicationNewsletterResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `creator_id` | `str` | Optional | - |
| `description` | `str` | Optional | - |
| `id` | `str` | Optional | - |
| `image` | `str` | Optional | - |
| `name` | `str` | Optional | - |
| `slug` | `str` | Optional | - |
| `subscribers` | `int` | Optional | - |

## Example

```python
from mediumapi.models.publication_newsletter_response import PublicationNewsletterResponse

publication_newsletter_response = PublicationNewsletterResponse(
    creator_id='aea8a19ea239',
    description='We have moved our newsletter. Subscribe → https://ws.towardsai.net/subscribe',
    id='d710a73cd042',
    image='https://miro.medium.com/1*j2OVd7j2o2FHeE7T8TzpXw.png',
    name='This AI newsletter is all you need',
    slug='this-ai-newsletter-is-all-you-need',
    subscribers=6752
)
```

