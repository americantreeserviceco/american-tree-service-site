# Security Policy

## Supported Versions

We actively maintain the `dev` branch as our staging environment and the `main` branch for deployment. Security updates are applied directly to the active operational tracks of this site.

| Version / Branch | Supported          | Notes |
| ---------------- | ------------------ | ----- |
| dev              | :white_check_mark: | Active development & staging environment |
| main             | :white_check_mark: | Production website deployment |
| Legacy / Archive | :x:                | Older static instances are not maintained |

## Reporting a Vulnerability

We take the security of our website, our automated arborist web scrapers, and our customer data very seriously. If you find a security vulnerability, please do not open a public GitHub issue. Instead, report it privately so we can fix it before it is exposed.

### How to Report

Please report security vulnerabilities by emailing our technical team directly:
* **Email:** security@americantreeserviceco.com
* **Subject Line:** `VULNERABILITY REPORT - [Brief Description]`

To help us resolve the issue quickly, please include:
1. A detailed description of the vulnerability.
2. Step-by-step instructions or a Proof of Concept (PoC) script to reproduce the issue.
3. The potential impact (e.g., exposing client details, bypassing forms, database vulnerabilities).

### What to Expect

* **Acknowledgement:** You will receive an initial response within **48 hours** confirming that we have received your report.
* **Updates:** We will provide status updates at least once every **3 to 5 business days** while we investigate and work on a patch.
* **Resolution:** If the vulnerability is accepted, we will coordinate a fix and deploy it to the `dev` and `main` branches. We will notify you as soon as the patch is live.

### Scope of Interest

We are primarily concerned with vulnerabilities that could compromise:
* Customer data submitted via quote request forms or appointment schedulers.
* Exposed credentials or API keys within our JavaScript files or GitHub Actions environment secrets (`TWILIO_AUTH_TOKEN`, Supabase service keys, etc.).
* Code injection points in the standalone blog creator tool.
