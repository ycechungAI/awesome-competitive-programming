## 2026-02-02 - HTTPS Availability on Legacy CP Sites
**Vulnerability:** Insecure HTTP links in documentation.
**Learning:** `e-maxx.ru` and potentially other older Russian/Asian competitive programming archives do not support HTTPS or have invalid certificates. Upgrading them blindly breaks the links.
**Prevention:** Verify SSL support manually or via `curl` before batch upgrading links for legacy sites.

## 2024-04-02 - Mass Unencrypted Connection (HTTP) Upgrade to HTTPS
**Vulnerability:** Many links in the README.md and index.md reference HTTP URLs which could leak user activity over unencrypted channels or be subject to MITM attacks leading to malicious content substitution.
**Learning:** Legacy competitive programming websites referenced in the project (e.g., e-maxx.ru, algorithmic tutorials) may not support HTTPS, but many others (especially academic sites and modern platforms) do now. Upgrading these links manually ensures safer browsing for readers.
**Prevention:** Always verify if a site supports HTTPS and use it by default when adding new resources.
