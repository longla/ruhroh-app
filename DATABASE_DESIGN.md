# Database Design

Based on the application requirements, here is a proposed database schema.

## Schema

*   **users**
    *   `id` (Primary Key, UUID)
    *   `email` (varchar, unique)
    *   `password_hash` (varchar)
    *   `role` (enum: `sitter`, `business_owner`)
    *   `created_at` (timestamp)
    *   `updated_at` (timestamp)

*   **sitters**
    *   `user_id` (Foreign Key to users.id, Primary Key)
    *   `rate` (decimal)
    *   `discount` (decimal)

*   **pets**
    *   `id` (Primary Key, UUID)
    *   `name` (varchar)
    *   `breed` (varchar)
    *   `age` (integer)
    *   `special_needs` (text)
    *   `owner_name` (varchar)
    *   `owner_contact` (varchar)

*   **requests**
    *   `id` (Primary Key, UUID)
    *   `pet_id` (Foreign Key to pets.id)
    *   `start_date` (timestamp)
    *   `end_date` (timestamp)
    *   `status` (enum: `pending`, `assigned`, `accepted`, `declined`, `completed`)
    *   `assigned_sitter_id` (Foreign Key to users.id, nullable)
    *   `created_at` (timestamp)
    *   `updated_at` (timestamp)

*   **request_sitter_assignments**
    *   `request_id` (Foreign Key to requests.id)
    *   `sitter_id` (Foreign Key to users.id)
    *   `status` (enum: `pending`, `accepted`, `declined`)
    *   Primary Key (`request_id`, `sitter_id`)
