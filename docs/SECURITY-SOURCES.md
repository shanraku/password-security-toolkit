# Security reference sources

Curated starting points for password and account security. Prefer current official guidance and review links periodically.

| Source | Purpose |
|---|---|
| [NIST SP 800-63 Digital Identity Guidelines](https://pages.nist.gov/800-63-4/) | Digital identity and authenticator guidance |
| [CISA Secure Our World](https://www.cisa.gov/secure-our-world) | Practical account and MFA security |
| [OWASP Authentication Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html) | Application authentication practices |
| [Have I Been Pwned Pwned Passwords](https://haveibeenpwned.com/Passwords) | Known compromised password corpus |
| [Have I Been Pwned API](https://haveibeenpwned.com/API/v3#PwnedPasswords) | Range API and k-anonymity documentation |

## Live data and refresh behavior
The optional breach checker queries the Pwned Passwords range API only after a user action. The public reference list is bundled with the app; it is not silently refreshed in the background. A static GitHub Pages deployment has no always-running scheduler. A future scheduled workflow may validate source availability and refresh a timestamped index, but must not collect passwords or user data.

Always check each source's current terms, rate limits and published guidance before integrating it.
