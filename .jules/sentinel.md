## 2025-02-01 - [Hardcoded Placeholder API Key]
**Vulnerability:** A hardcoded placeholder string `PLACEHOLDER_API_KEY` was used for the Gemini API client, preventing functionality and potentially encouraging users to hardcode secrets.
**Learning:** Even client-side apps need a strategy for secrets. "Bring Your Own Key" (BYOK) via LocalStorage is a valid pattern for static sites where no backend exists to proxy requests.
**Prevention:** Always implement a configuration loading mechanism (like reading from environment variables or LocalStorage) instead of placeholders, especially for authentication tokens.
