# Article

```python
article_controller = client.article
```

## Class Name

`ArticleController`

## Methods

* [Get Article Info](../../doc/controllers/article.md#get-article-info)
* [Get Article S Content](../../doc/controllers/article.md#get-article-s-content)
* [Get Article Fans](../../doc/controllers/article.md#get-article-fans)
* [Get Article S Markdown](../../doc/controllers/article.md#get-article-s-markdown)
* [Get Related Articles](../../doc/controllers/article.md#get-related-articles)
* [Get Article Responses](../../doc/controllers/article.md#get-article-responses)


# Get Article Info

Returns the article related information such as *Title, Subtitle, Tags,  Topics* (assigned by Medium), *Publication, Published date and time,  Clap Count, Voter Count, Word Count, Reading Time, Language, etc…*

:information_source: **Note** This endpoint does not require authentication.

```python
def get_article_info(self,
                    article_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `article_id` | `str` | Template, Required | It's a unique hash id assigned to every Medium Article. |

## Response Type

**200**: OK

[`ArticleResponse`](../../doc/models/article-response.md)

## Example Usage

```python
article_id = 'f06086080568'

result = article_controller.get_article_info(article_id)
print(result)
```


# Get Article S Content

Returns the content of an article/story, for the corresponding `article_id`

:information_source: **Note** This endpoint does not require authentication.

```python
def get_article_s_content(self,
                         article_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `article_id` | `str` | Template, Required | It's a unique hash id assigned to every Medium Article. |

## Response Type

**200**: OK

[`ArticleContentResponse`](../../doc/models/article-content-response.md)

## Example Usage

```python
article_id = '562c5821b5f0'

result = article_controller.get_article_s_content(article_id)
print(result)
```


# Get Article Fans

Returns a list of `user_ids` of the people who clapped on the article (a.k.a `voters`).

:information_source: **Note** This endpoint does not require authentication.

```python
def get_article_fans(self,
                    article_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `article_id` | `str` | Template, Required | It's a unique hash id assigned to every Medium Article. |

## Response Type

**200**: OK

[`ArticleFansResponse`](../../doc/models/article-fans-response.md)

## Example Usage

```python
article_id = '67fa62fc1971'

result = article_controller.get_article_fans(article_id)
print(result)
```


# Get Article S Markdown

Returns the markdown of an article/story from Medium, for the corresponding `article_id`

:information_source: **Note** This endpoint does not require authentication.

```python
def get_article_s_markdown(self,
                          article_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `article_id` | `str` | Template, Required | It's a unique hash id assigned to every Medium Article. |

## Response Type

**200**: OK

[`ArticleMarkdownResponse`](../../doc/models/article-markdown-response.md)

## Example Usage

```python
article_id = '67fa62fc1971'

result = article_controller.get_article_s_markdown(article_id)
print(result)
```


# Get Related Articles

Returns a list of `article_ids` of the related posts. (Length = 5)

**Note:** If the given article is self-published, related posts will belong to the same author,  else related posts will belong to the publication in which the article is published.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_related_articles(self,
                        article_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `article_id` | `str` | Template, Required | It's a unique hash id assigned to every Medium Article. |

## Response Type

**200**: OK

[`ArticleRelatedResponse`](../../doc/models/article-related-response.md)

## Example Usage

```python
article_id = '67fa62fc1971'

result = article_controller.get_related_articles(article_id)
print(result)
```


# Get Article Responses

Returns a list of responses (`response_ids`, same as `article_ids`) for a given article (`article_id`)
Note: To see the content of the response, use the "Get Article's Content" endpoint

:information_source: **Note** This endpoint does not require authentication.

```python
def get_article_responses(self,
                         article_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `article_id` | `str` | Template, Required | It's a unique hash id assigned to every Medium Article. |

## Response Type

**200**: OK

[`ArticleResponsesResponse`](../../doc/models/article-responses-response.md)

## Example Usage

```python
article_id = '67fa62fc1971'

result = article_controller.get_article_responses(article_id)
print(result)
```

