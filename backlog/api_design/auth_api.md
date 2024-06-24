API Design: Authentication
==========================

Register User
-------------

- **Endpoint:** `POST /auth/register`
- **Description:** Registers a new user.
- **Request Body:**
    {
      "username": "string",
      "email": "string",
      "password": "string"
    }
- **Response:**
    {
      "id": "string",
      "username": "string",
      "email": "string"
    }

Login User
----------

- **Endpoint:** `POST /auth/login`
- **Description:** Logs in a user.
- **Request Body:**
    {
      "email": "string",
      "password": "string"
    }
- **Response:**
    {
      "accessToken": "string"
    }

Get User Profile
----------------

- **Endpoint:** `GET /users/profile`
- **Description:** Retrieves the profile of the logged-in user.
- **Response:**
    {
      "id": "string",
      "username": "string",
      "email": "string"
    }

Social Login via LINE
---------------------

- **Endpoint:** `GET /auth/line`
- **Description:** Redirects user to LINE for authentication.
- **Response:** Redirects to LINE login page.

LINE Callback
-------------

- **Endpoint:** `GET /auth/line/callback`
- **Description:** Handles the callback from LINE after authentication.
- **Response:**
    {
      "accessToken": "string",
      "user": {
        "id": "string",
        "username": "string",
        "email": "string"
      }
    }

Social Login via Facebook
-------------------------

- **Endpoint:** `GET /auth/facebook`
- **Description:** Redirects user to Facebook for authentication.
- **Response:** Redirects to Facebook login page.

Facebook Callback
-----------------

- **Endpoint:** `GET /auth/facebook/callback`
- **Description:** Handles the callback from Facebook after authentication.
- **Response:**
    {
      "accessToken": "string",
      "user": {
        "id": "string",
        "username": "string",
        "email": "string"
      }
    }

Social Login via Google
-----------------------

- **Endpoint:** `GET /auth/google`
- **Description:** Redirects user to Google for authentication.
- **Response:** Redirects to Google login page.

Google Callback
---------------

- **Endpoint:** `GET /auth/google/callback`
- **Description:** Handles the callback from Google after authentication.
- **Response:**
    {
      "accessToken": "string",
      "user": {
        "id": "string",
        "username": "string",
        "email": "string"
      }
    }
