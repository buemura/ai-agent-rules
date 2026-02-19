# Rules for secrets management

## This file describes the rules for managing secrets in the project.

Secrets such as API keys, database credentials, and other sensitive information should never be hardcoded in the codebase. Instead, they should be stored securely using environment variables (`.env` files). Ensure that secrets are encrypted at rest and in transit, and that access to them is restricted to only those who need it. Additionally, secrets should be rotated regularly to minimize the risk of unauthorized access.

Projects should have a `.env.example` file that lists all the required environment variables without actual values, serving as a template for developers to create their own `.env` files. This helps maintain consistency and ensures that all necessary secrets are accounted for.

Each project should have its own `.env` file that is not committed to version control, containing the actual values for the secrets. This file should be included in the `.gitignore` file to prevent it from being accidentally committed to the repository. Developers should be instructed to create their own `.env` files based on the `.env.example` template and to keep their secrets secure.
