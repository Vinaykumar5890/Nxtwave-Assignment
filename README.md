# Todo Application

Given an `app.js` file and an empty database file `contact.db`.

Create a table with the name `todo` with the following columns,

**Todo Table**

| Column   | Type    |
| -------- | ------- |
| id       | VARCHAR |
| name     | VARCHAR |
| email    | VARCHAR |
| contact  | VARCHAR |

and write APIs to perform operations on the table `contacts`,


### API 1

#### Path: `/contacts/`

#### Method: `GET`

  - **Description**:

    Returns a list of all Contacts 

  - **Response**

    ```
    [
      {
        id: 4,
        name: "Play volleyball",
        email: "MEDIUM@gmail.com",
       contact: "90404958475"
      },
      ...
    ]
    ```

### API 2

#### Path: `/contacts/:id/`

#### Method: `GET`

#### Description:

Returns a specific contact based on the  ID

#### Response

```
{
  id: 2,
  name: "Learn JavaScript",
  email: "HIGH@gmail.com",
  contact: "85694896479"
}
```

### API 3

#### Path: `/contacts/`

#### Method: `POST`

#### Description:

Create a contacts in the todo table,

#### Request

```
{
  "id": 10,
  "name": "Finalize event theme",
  "email": "LOW@gmail.com",
  "contact": "857946798"
}
```

#### Response

```
Contact Successfully Added
```

### API 4

#### Path: `/contacts/:id/`

#### Method: `PUT`

#### Description:

Updates the details of a specific contact based on the  ID

  - **Request**
    ```
    {
      "name: "yadava"
    }
    ```
  - **Response**

    ```
    Contact  Updated Succesfully
    ```

### API 5

#### Path: `/contacts/:id/`

#### Method: `DELETE`

#### Description:

Deletes a contact from the based on the contact ID

#### Response

```
Contact Deleted Succesfully
```

<br/>

Use `npm install` to install the packages.

**Export the express instance using the default export syntax.**

**Use Common JS module syntax.**
