<p align="center">
  <a href="#" target="_blank">
    <img src="https://github.com/meilisearch/meilisearch/blob/main/assets/logo.svg" alt="Meilisearch" width="200" height="200" />
  </a>
</p>

<h1 align="center">WebGL Three.js Nuxt 3 ecommerce demo</h1>

<p align="center">
  <a href="https://github.com/meilisearch/demo-movies/blob/main/LICENCE"><img src="https://img.shields.io/badge/license-MIT-informational" alt="License"></a>
</p>
<br/>

## 💪 Looking to build this yourself?

Read our [Step by step guide to adding site search to your Nuxt ecommerce]!

## 🧰 Stack

This project requires:

- [Node 18](https://nodejs.org/)
- [Yarn](https://classic.yarnpkg.com/) — Node.js packages manager
- [Nuxt 3](https://nuxt.com) — Web application framework based on [Vue 3](https://vuejs.org/)

This projects uses icons from [Heroicons] and social medias icons from [icons8](https://icons8.com/icons/collections/EnE9mEHAiX2D).

## 🛠️ Setup

### Dependencies

> **Warning**
> Ensure that you are using a Node version compatible with the one in `.nvmrc`.

Install the dependencies with Yarn:

```bash
yarn install
```

### Environment

Environment variables should hold your Meilisearch database credentials. The easiest way to launch a database is to [create a free project] on Meilisearch Cloud. Alternatively, you can read [local installation] documentation for self-hosted options.

This project loads environment variables from an `.env` file. You can duplicate the existing `.env.example` file and rename it as `.env`. Update the content of the file to match your credentials.

```bash
# .env

# Meilisearch configuration
MEILISEARCH_HOST="use the Database URL here"
MEILISEARCH_ADMIN_API_KEY="use the Default Admin API Key here"
MEILISEARCH_SEARCH_API_KEY="use the Default Search API Key here"

# Image optimization configuration
TWICPICS_DOMAIN=https://meilisearch-ecommerce.twic.pics
STORYBOOK_TWICPICS_DOMAIN=https://meilisearch-ecommerce.twic.pics
```

> This application uses [TwicPics] to deliver optimized images. You don’t need to update the related environment variables. 

### Database

Run the setup script to configure and seed your Meilisearch instance:

```bash
yarn setup
```

## 🧑‍💻 Development

> **Note**
> Make sure to complete instructions from the Setup section before running the server.

Start the development server on http://localhost:3000

```bash
yarn dev
```

## 🚀 Deployment

Build the application for production:

```bash
yarn build
```

Locally preview production build:

```bash
yarn preview
```

Check out the [deployment documentation] for more information.

## ✨ Storybook

This project uses [Storybook v7](https://storybook.js.org/) to document components. The `vite.config.ts` is used by Storybook to enable auto-imports and path aliases.

Open Storybook by running:

```bash
yarn storybook
```

> Output files `auto-imports.d.ts` and `components.d.ts` are auto-generated and *should not* be updated manually. You can commit them into source control.

