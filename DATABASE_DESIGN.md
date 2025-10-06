# Database Design

Based on the application requirements, here is a proposed database schema.

## Schema

*   **users**
    *   `id` (Primary Key, UUID)
    *   `username` (varchar, unique)
    *   `password_hash` (varchar)
    *   `profile_picture_url` (varchar)
    *   `bio` (text)
    *   `created_at` (timestamp)
    *   `updated_at` (timestamp)

*   **friendships**
    *   `user_id_1` (Foreign Key to users.id)
    *   `user_id_2` (Foreign Key to users.id)
    *   `status` (enum: `pending`, `accepted`)
    *   `created_at` (timestamp)
    *   `updated_at` (timestamp)
    *   Primary Key (`user_id_1`, `user_id_2`)

*   **posts**
    *   `id` (Primary Key, UUID)
    *   `user_id` (Foreign Key to users.id)
    *   `content` (text)
    *   `media_url` (varchar, optional)
    *   `created_at` (timestamp)
    *   `expires_at` (timestamp)

*   **reactions**
    *   `id` (Primary Key, UUID)
    *   `post_id` (Foreign Key to posts.id)
    *   `user_id` (Foreign Key to users.id)
    *   `emoji` (varchar)
    *   `created_at` (timestamp)
    *   Unique Constraint (`post_id`, `user_id`)

*   **crowns**
    *   `id` (Primary Key, UUID)
    *   `user_id` (Foreign Key to users.id)
    *   `week_start_date` (date)
    *   `created_at` (timestamp)
