# User

```python
user_controller = client.user
```

## Class Name

`UserController`

## Methods

* [Get User ID](../../doc/controllers/user.md#get-user-id)
* [Get User Info](../../doc/controllers/user.md#get-user-info)
* [Get User S Articles](../../doc/controllers/user.md#get-user-s-articles)
* [Get User Followers](../../doc/controllers/user.md#get-user-followers)
* [Get User Following](../../doc/controllers/user.md#get-user-following)
* [Get User S Interests](../../doc/controllers/user.md#get-user-s-interests)
* [Get User S Lists](../../doc/controllers/user.md#get-user-s-lists)
* [Get User S Publications](../../doc/controllers/user.md#get-user-s-publications)
* [Get User S Top Articles](../../doc/controllers/user.md#get-user-s-top-articles)


# Get User ID

Returns the unique `user_id` for the given `username`.

**Note:** You can find the `username` from the user's/author's profile page URL.

- **username**.medium.com
- medium.com/@**username**

:information_source: **Note** This endpoint does not require authentication.

```python
def get_user_id(self,
               username)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `username` | `str` | Template, Required | It's a unique string chosen by every single Medium user. |

## Response Type

**200**: OK

[`UserIdForResponse`](../../doc/models/user-id-for-response.md)

## Example Usage

```python
username = 'nishu-jain'

result = user_controller.get_user_id(username)
print(result)
```


# Get User Info

Returns user related information like *Full name, Bio, Followers count, Following count, Twitter username, Profile-image URL, User ID, etc...*

It takes `user_id` as the path parameter.

**Note:** If you don't know the `user_id`, then you can get it from the endpoint\
'/user/id_for/{`username`}'.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_user_info(self,
                 user_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `user_id` | `str` | Template, Required | It's a unique hash id assigned to every single Medium user. |

## Response Type

**200**: OK

[`UserResponse`](../../doc/models/user-response.md)

## Example Usage

```python
user_id = '1985b61817c3'

result = user_controller.get_user_info(user_id)
print(result)
```


# Get User S Articles

Returns the list of articles (`article_ids`) written by the user.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_user_s_articles(self,
                       user_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `user_id` | `str` | Template, Required | Unique hash id assigned to every single Medium user. |

## Response Type

**200**: OK

[`UserArticlesResponse`](../../doc/models/user-articles-response.md)

## Example Usage

```python
user_id = '1985b61817c3'

result = user_controller.get_user_s_articles(user_id)
print(result)
```


# Get User Followers

Returns the list of `user_ids` of the user's followers.

**Note:** The length of this followers' list might be different from what you get in  the "Get User Info" Endpoint. It's because, this list doesn't include Medium Users who  left the platform.
If you really need the exact followers' count, use this endpoint to get the followers'  list and take its length as the exact followers' count

:information_source: **Note** This endpoint does not require authentication.

```python
def get_user_followers(self,
                      user_id,
                      count=None)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `user_id` | `str` | Template, Required | Unique hash id assigned to every single Medium user. |
| `count` | `int` | Query, Optional | To limit the number of results. (count &lt; 1500) |

## Response Type

**200**: OK

[`UserFollowersResponse`](../../doc/models/user-followers-response.md)

## Example Usage

```python
user_id = '1985b61817c3'

count = 10

result = user_controller.get_user_followers(
    user_id,
    count=count
)
print(result)
```


# Get User Following

Returns the list of `user_ids` of the user's followings.

**Note:** Currently, this list does not contain the `publication_ids` of the publications that the user is following.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_user_following(self,
                      user_id,
                      count=None)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `user_id` | `str` | Template, Required | Unique hash id assigned to every single Medium user. |
| `count` | `int` | Query, Optional | To limit the number of results. (count &lt; 1500) |

## Response Type

**200**: OK

[`UserFollowingResponse`](../../doc/models/user-following-response.md)

## Example Usage

```python
user_id = '14d5c41e0264'

count = 10

result = user_controller.get_user_following(
    user_id,
    count=count
)
print(result)
```


# Get User S Interests

Returns a list of tags that the given user follows.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_user_s_interests(self,
                        user_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `user_id` | `str` | Template, Required | Unique hash id assigned to every single Medium user. |

## Response Type

**200**: OK

[`UserInterestsResponse`](../../doc/models/user-interests-response.md)

## Example Usage

```python
user_id = '1985b61817c3'

result = user_controller.get_user_s_interests(user_id)
print(result)
```


# Get User S Lists

Returns an array of `list_ids` created by the user.

**Note:** You can check whether the use has created lists or not beforehand. Check the  `has_list` attribute in the "Article Info" endpoint.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_user_s_lists(self,
                    user_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `user_id` | `str` | Template, Required | Unique hash id assigned to every single Medium user. |

## Response Type

**200**: OK

[`UserListsResponse`](../../doc/models/user-lists-response.md)

## Example Usage

```python
user_id = '5142451174a3'

result = user_controller.get_user_s_lists(user_id)
print(result)
```


# Get User S Publications

Returns a list of `publication_ids` where the user is the editor and/or creator.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_user_s_publications(self,
                           user_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `user_id` | `str` | Template, Required | Unique hash id assigned to every single Medium user. |

## Response Type

**200**: OK

[`UserPublicationsResponse`](../../doc/models/user-publications-response.md)

## Example Usage

```python
user_id = '14d5c41e0264'

result = user_controller.get_user_s_publications(user_id)
print(result)
```


# Get User S Top Articles

Returns a list of `article_ids` of the top 10 articles on the user's profile, for a given `user_id`.

:information_source: **Note** This endpoint does not require authentication.

```python
def get_user_s_top_articles(self,
                           user_id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `user_id` | `str` | Template, Required | Unique hash id assigned to every single Medium user. |

## Response Type

**200**: OK

[`UserTopArticlesResponse`](../../doc/models/user-top-articles-response.md)

## Example Usage

```python
user_id = '1985b61817c3'

result = user_controller.get_user_s_top_articles(user_id)
print(result)
```

