# Rule for API deployment

## This rule applies to Backend project deployment.

API should be containerized using Docker to ensure consistency across different environments. The Dockerfile should be well-structured and optimized for performance, including multi-stage builds to reduce the final image size.Additionally, the deployment should be configured to use environment variables for sensitive information such as database credentials and API keys, ensuring that these values are not hardcoded in the codebase.
