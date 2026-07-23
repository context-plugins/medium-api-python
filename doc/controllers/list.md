# List

```python
list_controller = client.list
```

## Class Name

`ListController`

## Methods

* [Get List Info](../../doc/controllers/list.md#get-list-info)
* [Get List Articles](../../doc/controllers/list.md#get-list-articles)
* [Get List Responses](../../doc/controllers/list.md#get-list-responses)


# Get List Info

Returns the list-related information such as *id, name, author, description,  thumbnail image url, creation datetime, last article inserted datetime,  number of articles in the list, claps, voters, and comments/responses*.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_list_info(self,
                 list_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `list_id` | `str` | Template, Required | It's a unique hash id assigned to every Medium List. |

## Response Type

**200**: OK

[`ListResponse`](../../doc/models/list-response.md)

## Example Usage

```python
list_id = '38f9e0f9bea6'

result = list_controller.get_list_info(list_id)
print(result)
```


# Get List Articles

Returns an array of `articles_ids` present in the given Medium List.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_list_articles(self,
                     list_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `list_id` | `str` | Template, Required | It's a unique hash id assigned to every Medium List. |

## Response Type

**200**: OK

[`ListArticlesResponse`](../../doc/models/list-articles-response.md)

## Example Usage

```python
list_id = '38f9e0f9bea6'

result = list_controller.get_list_articles(list_id)
print(result)
```


# Get List Responses

Returns an array of `response_ids` of the comments (same as `article_ids`) on the given Medium List.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_list_responses(self,
                      list_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `list_id` | `str` | Template, Required | It's a unique hash id assigned to every Medium List. |

## Response Type

**200**: OK

[`ListResponsesResponse`](../../doc/models/list-responses-response.md)

## Example Usage

```python
list_id = '38f9e0f9bea6'

result = list_controller.get_list_responses(list_id)
print(result)
```

