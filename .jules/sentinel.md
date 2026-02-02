## 2026-02-02 - HTTPS Availability on Legacy CP Sites
**Vulnerability:** Insecure HTTP links in documentation.
**Learning:** `e-maxx.ru` and potentially other older Russian/Asian competitive programming archives do not support HTTPS or have invalid certificates. Upgrading them blindly breaks the links.
**Prevention:** Verify SSL support manually or via `curl` before batch upgrading links for legacy sites.
