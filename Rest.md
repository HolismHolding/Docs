# REST

<br />
<br />

## World's formula

|        | HTTP method |    URL   |      URL parameters      | Request body | Response body |
|--------|:-----------:|:--------:|:------------------------:|:------------:|:-------------:|
| Create |     POST    |   Items  |                          |   item JSON  |               |
| Read   |     GET     |   Items  | filter, sort, pagination |              |               |
| Update |     PUT     | Items/Id |                          |   item JSON  |               |
| Delete |    DELETE   | Items/Id |                          |              |               |

<br />
<br />
<br />
<br />

## Holism's formula

|        | HTTP method |       URL      |      URL parameters      | Request body | Response body |
|--------|:-----------:|:--------------:|:------------------------:|:------------:|:-------------:|
| Create |     POST    |   Item/Create  |                          |   item JSON  |               |
| Read   |     GET     |    Item/List   | filter, sort, pagination |              |               |
| Update |     POST    | Item/Update/Id |                          |   item JSON  |               |
| Delete |     POST    | Item/Delete/Id |                          |              |               |
| Upsert |     POST    |  Item/Upsert   |                          |   item JSON  |               |

<br />
<br />
<br />

### Notes

- If action is:
    - Read
        - HTTP verb/method = `GET`
    - Write
        - HTTP verb/method = `POST`
- We don't use `PUT` or `DELETE` or other HTTP Verbs/Methods
- URL naming = `entity/action/:id?:params`
- Action names are verbs
