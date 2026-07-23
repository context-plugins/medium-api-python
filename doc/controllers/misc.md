# Misc

```python
misc_controller = client.misc
```

## Class Name

`MiscController`

## Methods

* [Get Latest Posts](../../doc/controllers/misc.md#get-latest-posts)
* [Get Related Tags](../../doc/controllers/misc.md#get-related-tags)
* [Get Top Writers](../../doc/controllers/misc.md#get-top-writers)
* [Get Topfeeds](../../doc/controllers/misc.md#get-topfeeds)


# Get Latest Posts

Returns a list of latest posts (`article_ids`) for a topic/niche (as classified by the Medium platform). Example of a topic/niche can be:

* blockchain
* relationships
* mental-health, etc …

These are known as `topic_slugs`. At any given moment, this endpoint will return a list of 25 articles (`article_ids`).

:information_source: **Note** This endpoint does not require authentication.

```python
def get_latest_posts(self,
                    topic_slug)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `topic_slug` | `str` | Template, Required | It's a unique string, usually hyphen-separated, representing a topic/niche, as classified by Medium. |

## Response Type

**200**: OK

[`LatestpostsResponse`](../../doc/models/latestposts-response.md)

## Example Usage

```python
topic_slug = 'artificial-intelligence'

result = misc_controller.get_latest_posts(topic_slug)
print(result)
```


# Get Related Tags

Returns a list of `related_tags` for the given `tag`.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_related_tags(self,
                    tag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `tag` | `str` | Template, Required | It's a unique string, usually hyphen-separated, representing a class of content. |

## Response Type

**200**: OK

[`RelatedTagsResponse`](../../doc/models/related-tags-response.md)

## Example Usage

```python
tag = 'blockchain'

result = misc_controller.get_related_tags(tag)
print(result)
```


# Get Top Writers

Returns a list of top writers (`user_ids`) within a particular topic/niche (`topic_slug`).
e.g.

- blockchain
- relationships
- artificial-intelligence, etc ...

**Note:** You can use optional `count` query parameter to limit the number of results.  The maximum number of top writers within a topic/niche will be 250.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_top_writers(self,
                   topic_slug,
                   count=None)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `topic_slug` | `str` | Template, Required | It's a unique string, usually hyphen-separated, representing a topic/niche, as classified by Medium. |
| `count` | `int` | Query, Optional | Limits the number of `article_ids` in the result. |

## Response Type

**200**: OK

[`TopWriterResponse`](../../doc/models/top-writer-response.md)

## Example Usage

```python
topic_slug = 'relationships'

count = 10

result = misc_controller.get_top_writers(
    topic_slug,
    count=count
)
print(result)
```


# Get Topfeeds

Returns a list of `article_ids` (length: 25) for the given `tag` and `mode`.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_topfeeds(self,
                tag,
                mode,
                after=0,
                count=25)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `tag` | `str` | Template, Required | It's a unique string, usually hyphen-separated, representing a class of content. |
| `mode` | `str` | Template, Required | Mode:<br><br>- `hot` : For getting trending articles<br>- `new` : For getting latest articles<br>- `top_year` : For getting best articles of the year<br>- `top_month` : For getting best articles of the month<br>- `top_week` : For getting best articles of the week<br>- `top_all_time`: For getting best article of all time |
| `after` | `int` | Query, Optional | To get the subsequent top feeds. (`after` &lt; 250)<br><br>**Default**: `0` |
| `count` | `int` | Query, Optional | To limit the number of top feeds. (`count` &lt; 25)<br><br>**Default**: `25` |

## Response Type

**200**: OK

[`TopfeedsResponse`](../../doc/models/topfeeds-response.md)

## Example Usage

```python
tag = 'artificial-intelligence'

mode = 'new'

after = 10

count = 20

result = misc_controller.get_topfeeds(
    tag,
    mode,
    after=after,
    count=count
)
print(result)
```

