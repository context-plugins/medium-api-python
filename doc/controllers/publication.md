# Publication

```python
publication_controller = client.publication
```

## Class Name

`PublicationController`

## Methods

* [Get Publication ID](../../doc/controllers/publication.md#get-publication-id)
* [Get Publication Info](../../doc/controllers/publication.md#get-publication-info)
* [Get Publication Articles](../../doc/controllers/publication.md#get-publication-articles)
* [Get Publication Newsletter](../../doc/controllers/publication.md#get-publication-newsletter)


# Get Publication ID

Returns the unique `publication_id` for the given `publication_slug`.

**Note:** You can find the `publication_slug` from the publication's homepage URL.

- medium.com/**publication_slug**

:information_source: **Note** This endpoint does not require authentication.

```python
def get_publication_id(self,
                      publication_slug)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `publication_slug` | `str` | Template, Required | It's a lowercased hyphen-separated unique string alloted to each Medium Publication. |

## Response Type

**200**: OK

[`PublicationIdForResponse`](../../doc/models/publication-id-for-response.md)

## Example Usage

```python
publication_slug = 'codex'

result = publication_controller.get_publication_id(publication_slug)
print(result)
```


# Get Publication Info

Returns the publication related information such as *Publication name, Tagline, Description, Tags, Followers Count, Twitter username, Instagram username, Facebook Page name, etc …*

**Note:** If you don't know the `publication_id`, you can get it from any article published by it. Use endpoint "/article/{article_id}" to retrieve the `publication_id`.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_publication_info(self,
                        publication_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `publication_id` | `str` | Template, Required | It's a unique hash id assigned to every Medium Publication. |

## Response Type

**200**: OK

[`PublicationResponse`](../../doc/models/publication-response.md)

## Example Usage

```python
publication_id = '98111c9905da'

result = publication_controller.get_publication_info(publication_id)
print(result)
```


# Get Publication Articles

Returns the list of `articles_ids`, of the latest 25 articles, posted in that publication.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_publication_articles(self,
                            publication_id,
                            mfrom=None)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `publication_id` | `str` | Template, Required | It's a unique hash id assigned to every Medium Publication. |
| `mfrom` | `str` | Query, Optional | To get the articles before specified date and time. |

## Response Type

**200**: OK

[`PublicationArticlesResponse`](../../doc/models/publication-articles-response.md)

## Example Usage

```python
publication_id = '98111c9905da'

mfrom = '01/31/2023 13:10:00'

result = publication_controller.get_publication_articles(
    publication_id,
    mfrom=mfrom
)
print(result)
```


# Get Publication Newsletter

Returns the newsletter related information such as *id, name, description, slug, creator_id, subscribers, image_url, etc …*

**Note:** If you don't know the `publication_id`, you can get it from any article published by it. Use endpoint "/article/{article_id}" to retrieve the `publication_id`.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_publication_newsletter(self,
                              publication_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `publication_id` | `str` | Template, Required | It's a unique hash id assigned to every Medium Publication. |

## Response Type

**200**: OK

[`PublicationNewsletterResponse`](../../doc/models/publication-newsletter-response.md)

## Example Usage

```python
publication_id = '98111c9905da'

result = publication_controller.get_publication_newsletter(publication_id)
print(result)
```

