# Immutable Academics

Final year project. A system for issuing and verifying academic credentials (degrees, transcripts)
on the Ethereum blockchain so they can't be forged or tampered with.

## The problem

Fake degrees are a real issue. Verification is slow, manual, and relies on institutions responding
to requests. This makes credentials self-verifiable — anyone can check the on-chain hash against
the IPFS document.

## How it works

- Institutions issue credentials as transactions on Ethereum
- The actual documents (transcripts, marksheets) go on IPFS
- Verification = compare the on-chain hash with the IPFS content hash
- Frontend lets students view, share, and verify their records

## Stack

- **Frontend:** React + TypeScript + Vite, Tailwind CSS, shadcn/ui
- **Blockchain:** Ethereum (Ganache for local dev), Truffle for contract deployment
- **Storage:** IPFS for documents
- **Smart contracts:** Solidity

## Project structure

```
src/
  components/     # UI components
  contracts/      # Solidity ABIs and contract interfaces
  context/        # React context for Web3 connection
  pages/          # App views
  hooks/          # Custom hooks
  utils/          # Helpers
backend/
  contracts/      # Solidity source files
  migrations/     # Truffle deployment scripts
  truffle-config.js
```

## Related repo

The smart contract / Truffle side of this project is also at
[FP_Chain_edu](https://github.com/mrkrishna225/FP_Chain_edu).

## Run locally

```bash
git clone https://github.com/mrkrishna225/final-year-proj.git
cd final-year-proj
npm install
npm run dev
```

You'll need Ganache running for the blockchain backend.
