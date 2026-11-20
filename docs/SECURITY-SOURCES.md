# Security reference sources

Curated starting points for password and account security. Prefer current official guidance and review links periodically.

| Source | Purpose |
|---|---|
| [NIST SP 800-63 Digital Identity Guidelines](https://pages.nist.gov/800-63-4/) | Digital identity and authenticator guidance |
| [CISA Secure Our World](https://www.cisa.gov/secure-our-world) | Practical account and MFA security |
| [OWASP Authentication Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html) | Application authentication practices |
| [Have I Been Pwned Pwned Passwords](https://haveibeenpwned.com/Passwords) | Known compromised password corpus |
| [Have I Been Pwned API](https://haveibeenpwned.com/API/v3#PwnedPasswords) | Range API and k-anonymity documentation |

## Bitcoin references
- [Bitcoin.org — Secure your wallet](https://bitcoin.org/en/secure-your-wallet)
- [Bitcoin Core documentation](https://bitcoincore.org/en/doc/)
- [mempool.space](https://mempool.space/) — public Bitcoin mempool and block explorer
- [Blockstream Explorer](https://blockstream.info/) — public Bitcoin blockchain explorer

Explorers show public blockchain data; they cannot verify a recipient's identity or guarantee that a transaction is safe. Never submit recovery phrases or private keys to an explorer or third-party site.

## Live data and refresh behavior
The optional breach checker queries the Pwned Passwords range API only after a user action. The public reference list is bundled with the app; it is not silently refreshed in the background. A static GitHub Pages deployment has no always-running scheduler. A future scheduled workflow may validate source availability and refresh a timestamped index, but must not collect passwords or user data.

Always check each source's current terms, rate limits and published guidance before integrating it.
