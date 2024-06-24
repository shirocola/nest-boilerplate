Database Design
===============

1.  **Users Table:**

    -   `id`: UUID
    -   `username`: string
    -   `email`: string
    -   `password`: string (hashed)
    -   `created_at`: timestamp
    -   `updated_at`: timestamp
2.  **Products Table:**

    -   `id`: UUID
    -   `name`: string
    -   `description`: string
    -   `price`: number
    -   `image_url`: string
    -   `created_at`: timestamp
    -   `updated_at`: timestamp
3.  **Orders Table:**

    -   `id`: UUID
    -   `user_id`: UUID (foreign key to Users)
    -   `total_price`: number
    -   `created_at`: timestamp
    -   `updated_at`: timestamp
4.  **Order Items Table:**

    -   `id`: UUID
    -   `order_id`: UUID (foreign key to Orders)
    -   `product_id`: UUID (foreign key to Products)
    -   `quantity`: number
    -   `price`: number
    -   `created_at`: timestamp
    -   `updated_at`: timestamp