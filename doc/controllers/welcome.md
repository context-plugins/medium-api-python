# Welcome

```python
welcome_controller = client.welcome
```

## Class Name

`WelcomeController`


# Get Welcome

**Test Endpoint**
Returns the information about the Medium API

:information_source: **Note** This endpoint does not require authentication.

```python
def get_welcome(self)
```

## Response Type

**200**: OK

[`Response`](../../doc/models/response.md)

## Example Usage

```python
result = welcome_controller.get_welcome()
print(result)
```

