# Yessenov Campus — local Cloudflare Workers project

## Requirements
- Node.js LTS
- Git

## Run locally

```bash
npm install
npm run dev
```

Open the local URL printed by Wrangler (normally http://localhost:8787).

## Deploy to Cloudflare Workers

```bash
npx wrangler login
npm run deploy
```

## GitHub

Create an empty GitHub repository, then run these commands from this folder:

```bash
git init
git add .
git commit -m "Initial Yessenov Campus project"
git branch -M main
git remote add origin YOUR_GITHUB_REPOSITORY_URL
git push -u origin main
```

Then connect the repository in the Cloudflare dashboard under Workers & Pages → Create → Connect to Git. Choose this repository and deploy.

Note: the current page is a front-end demo. Login, WebAuthn/passkeys, and persistent student data are not connected yet; those will be implemented in the next development step with a backend and database.
