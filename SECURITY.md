# Security Policy

## What this repository contains

This repository publishes **only the built, ready-to-install extension package**
(`ixi-extension.zip`) together with documentation and screenshots. It is
deliberately kept free of anything sensitive:

- **No server or backend code.** The API, database and admin panel live in a
  separate, private repository and are never published here.
- **No credentials.** No database URLs, no API keys, no tokens, no signing
  secrets, no `.env` files.
- **No private keys.** No `.pem`, `.key` or certificate material of any kind.
- **No deploy access.** Nothing in this repository can deploy, roll back, or
  reach the admin panel.

## How the extension handles your data

- The extension runs entirely in your browser. It has **no server of its own**.
- It talks to exactly one host: **`https://ixiflower.vercel.app`** (plus
  `http://localhost:3000` for development builds of the site).
- Your session token is stored in the browser's own extension storage, on your
  machine. It is sent only to that site, and only to authenticate your own
  requests. It is never sent to any third party.
- Uninstalling the extension removes its stored data with it.

## Reporting a vulnerability

If you believe you've found a security issue, **please do not open a public
issue.** Instead, contact the maintainer privately:

- GitHub: [@Amirabbas-RU](https://github.com/Amirabbas-RU)

Please include a description of the issue, the steps to reproduce it, and any
relevant details. You'll get a response as soon as possible, and credit for the
report if you'd like it.

## Supported versions

Only the latest published version is supported. The extension's **Update**
panel tells you whether a newer build exists.
