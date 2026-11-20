# Password Security Toolkit

A free, privacy-first browser toolkit for generating random passwords, creating passphrases, estimating password strength, and optionally checking exposure in the Have I Been Pwned Pwned Passwords corpus.

## Features
- Cryptographically secure password generation using Web Crypto `crypto.getRandomValues()` and rejection sampling.
- Configurable length and character groups.
- Random passphrase generation.
- Local, approximate entropy estimate (not a security certification).
- Optional breach lookup using the Pwned Passwords range API and k-anonymity: only the first five hexadecimal characters of the SHA-1 hash are sent; the full hash and password are not sent.
- Curated links to NIST, CISA, OWASP and Have I Been Pwned.
- No account, backend, analytics or API key required.

## Bitcoin security
The Bitcoin section provides wallet, recovery-phrase, device, transaction and scam-safety guidance with links to Bitcoin.org, Bitcoin Core, mempool.space and Blockstream. It does not connect to wallets, request seed phrases or private keys, sign transactions, or provide investment advice. Block explorers expose public on-chain information and do not establish whether an address is trustworthy.

## Run locally
Open `index.html` from a static web server. For example:
```sh
python -m http.server 8000
```
Then visit `http://localhost:8000`. The optional breach lookup requires an internet connection and a browser that supports Web Crypto.

## Privacy and limitations
Password generation, passphrase generation and the strength estimate run in your browser. A breach lookup is only made after the user presses the check button. The app sends a five-character SHA-1 hash prefix to the Have I Been Pwned API; this is a privacy-preserving range lookup, not zero disclosure. The entered password is cleared from the field after the request. Do not paste a password into a device or browser you do not trust.

A negative breach result does not prove a password is safe. The strength score is a rough educational estimate and does not replace a password manager, unique passwords, or multi-factor authentication. Never reuse passwords.

## Sources and updates
The reference directory links to official standards and security guidance. The breach corpus is queried live on demand from Have I Been Pwned. This static site does not run a background scheduler; continuous automated source refresh would require a trusted scheduled workflow or hosting service. Source links and provider policies can change.

## Contributing
See [CONTRIBUTING.md](CONTRIBUTING.md). Please do not submit real passwords, secrets, or personal data in issues.

## Security
See [SECURITY.md](SECURITY.md). Please report vulnerabilities privately and never include live credentials.

## License
MIT. See [LICENSE](LICENSE).
