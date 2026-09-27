# Prediction Game

A Magic 8 Ball-style decentralized application built on the Nebulas blockchain in 2018.

> **Status:** Historical source only. [Nebulas ended its mainnet service](https://www.nebulas.io/) in December 2024, so the original interface can no longer retrieve answers from the deployed contract.

## How it worked

The smart contract initialized a map of short predictions. When the browser called `getResult`, the contract selected an answer and returned it to the page.

The lookup was read-only, so visitors did not need to unlock a wallet or submit a paid transaction simply to request an answer.

```text
Browser -> Nebulas read-only contract call -> prediction returned to the page
```

## Important files

- `magicEightBall.js` — original Nebulas smart contract and response list.
- `index.html` — original Magic 8 Ball interface and contract-call logic.
- `server.js` — small local static server used during development.
- `lib/` and `js/` — bundled Nebulas web-wallet dependencies.

## Technology

- JavaScript
- Nebulas smart contracts
- Nebulas JavaScript SDK
- HTML and CSS

## Historical note

This repository is preserved to document the contract design and early browser-to-blockchain integration. The bundled network and wallet libraries are obsolete and are not intended for current wallet use.
