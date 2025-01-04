# Umami Self-Hosted Analytics

## Getting Started

1.  **Clone the Repository:**

    ```bash
    git clone https://github.com/MLSAKIIT/umami.git
    cd umami
    ```

2.  **Configuration:**

    - Copy `.env.example` to `.env` and fill in the required environment variables.
    - Refer to the [Configuration](#configuration) documentation for details.

3.  **Deployment:**

    ```bash
    docker-compose up -d
    ```

4.  **Access Umami:**

    - Open your browser and navigate to `http://localhost:3000`.
    - Use the default login credentials: `admin:umami`.

### Configuration

For the configuration, you need to fill the following environment variables in the `.env` file, that are described in the `.env.example` file:

- `DATABASE_URL`: Connection string for your PostgreSQL Database
- `DATABASE_TYPE`: Must be set to `postgresql`
- `APP_SECRET`: A secret string used by Umami for security (Use `openssl rand -base64 32` to generate a strong string)
- `TRACKER_SCRIPT_NAME`: Optional Uncomment and change to have a custom name for the tracking script (e.g., `my_analytics_script`) to avoid ad-blockers.
- `POSTGRES_DB`: Name of the Database
- `POSTGRES_USER`: Name of the user
- `POSTGRES_PASSWORD`: Database password

### Troubleshooting

Refer to [umami docs](https://umami.is/docs)
