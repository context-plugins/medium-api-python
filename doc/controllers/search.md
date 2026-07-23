# Search

```python
search_controller = client.search
```

## Class Name

`SearchController`

## Methods

* [Search Articles](../../doc/controllers/search.md#search-articles)
* [Search Lists](../../doc/controllers/search.md#search-lists)
* [Search Publications](../../doc/controllers/search.md#search-publications)
* [Search Tags](../../doc/controllers/search.md#search-tags)
* [Search Users](../../doc/controllers/search.md#search-users)


# Search Articles

Returns the list of `articles_ids` for the given search query results. (Max Length = 1000)

:information_source: **Note** This endpoint does not require authentication.

```python
def search_articles(self,
                   query)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `query` | `str` | Template, Required | Search query |

## Response Type

**200**: OK

[`SearchArticlesResponse`](../../doc/models/search-articles-response.md)

## Example Usage

```python
query = 'startup'

result = search_controller.search_articles(query)
print(result)
```


# Search Lists

Returns an array of `list_ids` for the given search query results. (Max Length = 1000)

:information_source: **Note** This endpoint does not require authentication.

```python
def search_lists(self,
                query)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `query` | `str` | Template, Required | Search query |

## Response Type

**200**: OK

[`SearchListsResponse`](../../doc/models/search-lists-response.md)

## Example Usage

```python
query = 'artificial intelligence'

result = search_controller.search_lists(query)
print(result)
```


# Search Publications

Returns the list of `publication_ids` for the given search query results. (Max Length = 1000)

:information_source: **Note** This endpoint does not require authentication.

```python
def search_publications(self,
                       query)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `query` | `str` | Template, Required | Search query |

## Response Type

**200**: OK

[`SearchPublicationsResponse`](../../doc/models/search-publications-response.md)

## Example Usage

```python
query = 'mental health'

result = search_controller.search_publications(query)
print(result)
```


# Search Tags

Returns a list of `tags` for the given search query results. (Max Length = 1000)

:information_source: **Note** This endpoint does not require authentication.

```python
def search_tags(self,
               query)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `query` | `str` | Template, Required | Search query |

## Response Type

**200**: OK

[`SearchTagsResponse`](../../doc/models/search-tags-response.md)

## Example Usage

```python
query = 'blockchain'

result = search_controller.search_tags(query)
print(result)
```


# Search Users

Returns a list of `user_ids` for the given search query results. (Max Length = 1000)

:information_source: **Note** This endpoint does not require authentication.

```python
def search_users(self,
                query)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `query` | `str` | Template, Required | Search query |

## Response Type

**200**: OK

[`SearchUsersResponse`](../../doc/models/search-users-response.md)

## Example Usage

```python
query = 'data engineer'

result = search_controller.search_users(query)
print(result)
```

