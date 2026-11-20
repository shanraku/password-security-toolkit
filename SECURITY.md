# Security Policy

## Reporting
Please do not publish exploitable vulnerability details or real credentials in a public issue. Contact the repository owner through the GitHub profile and provide a concise description and reproduction steps without secrets.

## Security principles
- Passwords are generated locally with the Web Crypto API.
- Password strength estimation is local and approximate.
- Breach lookup is optional and user-initiated. It uses the Have I Been Pwned range endpoint: a five-character SHA-1 prefix is sent and matching suffixes are checked locally.
- Never send plaintext passwords, full hashes, or user-entered secrets to a server.
- External links open with `noopener noreferrer`.

## Scope and limitations
This project is an educational utility, not a certified password manager or security audit. A clean breach lookup is not proof that a password has never been exposed. Keep software and browsers updated and use a reputable password manager with multi-factor authentication.
