User Stories: Authentication
============================

User Registration and Authentication
------------------------------------

### As a User:

-   I want to register an account so that I can purchase bakery items.

    -   **Acceptance Criteria:**
        -   A user can register with a username, email, and password.
        -   The system should validate the email format and password strength.
        -   If the registration is successful, the user should receive a confirmation email.
-   I want to log in to my account so that I can view my order history and place new orders.

    -   **Acceptance Criteria:**
        -   A user can log in with an email and password.
        -   The system should provide an access token upon successful login.
        -   If the login fails, the user should receive an appropriate error message.

### As an Admin:

-   I want to manage user accounts so that I can ensure only authorized users can access certain features.
    -   **Acceptance Criteria:**
        -   Admins can view, update, and delete user accounts.
        -   Admin actions should be logged for audit purposes.

Social Login Integration
------------------------

### As a User:

-   I want to log in using my LINE, Facebook, or Google account so that I can easily access the bakery website without creating a new account.
    -   **Acceptance Criteria:**
        -   The system should redirect the user to the selected social media login page.
        -   Upon successful login, the system should create a new user account if one does not already exist.
        -   The system should log the user in and provide an access token.
        -   If the login fails, the user should receive an appropriate error message.

### As an Admin:

-   I want to manage users authenticated via social login to ensure proper access control.
    -   **Acceptance Criteria:**
        -   Admins can view users authenticated via social login.
        -   Admins can update or delete users authenticated via social login.
        -   Admin actions should be logged for audit purposes.