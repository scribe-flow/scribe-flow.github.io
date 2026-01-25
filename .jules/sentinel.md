# Sentinel's Journal

## 2025-02-18 - Placeholder Key Pattern & BYOK
**Vulnerability:** The application was using a hardcoded "PLACEHOLDER_API_KEY" which rendered the "Enhance & Fix" features non-functional without a way for users to supply their own key.
**Learning:** Static applications (JAMstack) often struggle with secret management. Hardcoding keys is bad, but placeholders that break functionality are also not ideal.
**Prevention:** Implement a "Bring Your Own Key" (BYOK) pattern using `localStorage` or session storage. This allows users to input their own credentials securely without the application owner hosting them.
