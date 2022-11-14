# Nuxt 3 Minimal Starter

Look at the [nuxt 3 documentation](https://v3.nuxtjs.org) to learn more.

## Setup

Make sure to install the dependencies:

```bash
# yarn
yarn install

# npm
npm install

# pnpm
pnpm install --shamefully-hoist
```

## Development Server

Start the development server on http://localhost:3000

```bash
npm run dev
```

## Production

Build the application for production:

```bash
npm run build
```

Locally preview production build:

```bash
npm run preview
```

During development, apps are usually served via HTTP. However, Storyblok v2 requires your app to be served via HTTPS. Please follow the steps below to enable this in a Nuxt 3 project.

Install mkcert on your system The installation instructions for macOS, Windows and Linux can be found in the mkcert Github repository.

Create a valid certificate by running the following command in your project folder:
mkcert localhost

In the project’s package.json, change the nuxt dev command to the following:
nuxt dev --https --ssl-cert localhost.pem --ssl-key localhost-key.pem

Run your project using npm run dev. Your project will now be served on https://localhost:3000.

Checkout the [deployment documentation](https://v3.nuxtjs.org/guide/deploy/presets) for more information.

/****\*\*****\*****\*\*****/
This project is a training project based on:

https://www.storyblok.com/tc/nuxtjs

storyblok account:

https://app.storyblok.com/#/me/spaces/179759/dashboard
