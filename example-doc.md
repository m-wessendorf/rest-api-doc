# Example API Documentation

Multiline description of the service and the api.

**Author:**<br>
John Doe :email: <john.doe@example.com>

**Icons:**<br>
:lock: Authentification required. <br>
:floppy_disk: Deprecated. <br>
:wrench: Only for testing. <br>
:new: New call. <br>
:sunrise_over_mountains: Images transmission.


## Profile example functionality

Create, edit and view a user profile.


<details>
  <summary><b>GET</b> <b><code>/profile/detail</code></b> - Get the public information on the profile.</summary>
  <br>

```
(Request)

URL-Params (Required): email=[String]
URL-Params (Optional): -

Data-Params: -
```
```
(Response)

Success-Response:
Code: 200
Content:
{
  name: [String],
  age: [int],
  description: [String]
}

Error-Response:
Code: 400 BAD REQUEST
Content: -

```
</details>

<br>

<details>
  <summary><b>GET</b> <b><code>/profile/all</code></b> :wrench: - Summary of all profiles.</summary>
  <br>

```
(Request)

URL-Params (Required): -
URL-Params (Optional): -

Data-Params: -
```
```
(Response)

Success-Response:
Code: 200
Content:
[
  {
    name: [String],
    age: [int]
  }
]

Error-Response:
Code: 400 BAD REQUEST
Content: -

```
</details>

<br>

<details>
  <summary><b>POST</b> <b><code>/profile/create</code></b> - Create a new profile.</summary>
  <br>

  ```
  (Request)

  URL-Params (Required): -
  URL-Params (Optional): -

  Data-Params:
  {
    name: [String],
    email: [String],
    age: [int],
    description: [String]
  }
  ```
  ```
  (Response)

  Success-Response:
  Code: 200
  Content: -

  Error-Response:
  Code: 400 BAD REQUEST
  Content: -

  ```

</details>
