# Immutable Academics

Final year project. A system for issuing and verifying academic credentials (degrees, transcripts)
on the Ethereum blockchain so they can't be forged or tampered with.

## The problem

Fake degrees are everywhere. Verification is slow, manual, and relies on trusting institutions
to respond to email requests. This project makes credentials self-verifiable.

## How it works

- Institutions issue credentials as transactions on Ethereum
- Document artifacts (transcripts, marksheets) are stored on IPFS
- Anyone can verify a credential by checking the on-chain hash against the IPFS document
- React + TypeScript frontend built with Vite, Tailwind, and shadcn/ui

## Stack

- Ethereum (Ganache for local dev, Truffle for deployment)
- IPFS for document storage
- React + TypeScript + Vite
- Tailwind CSS + shadcn/ui

## Related repo

[FP_Chain_edu](https://github.com/mrkrishna225/FP_Chain_edu) — the Truffle/Ganache contract deployment side of this project.

## Run locally

```bash
git clone https://github.com/mrkrishna225/final-year-proj.git
cd final-year-proj
npm install
npm run dev
```
