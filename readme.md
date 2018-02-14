## version

- [Lumen 5.4](https://github.com/laravel/lumen/tree/v5.4.0).

## Quick Start

- Clone this repo or download it's release archive and extract it somewhere
- You may delete `.git` folder if you get this code via `git clone`
- Run `composer install`
- Run `php artisan jwt:generate`
- Configure your `.env` file for authenticating via database
- Set the `API_PREFIX` parameter in your .env file (usually `api`).
- Run `php artisan migrate --seed`

## API Endpoint
  - [POST] /api/auth/login

    **Request:**
    ```
    {
        "email": "johndoe@example.com",
        "password": "johndoe"
    }
    ```

    **Response:**
    ```
    {
        "success": {
            "message": "token_generated",
            "token": [token_here]
        }
    }
    ```
