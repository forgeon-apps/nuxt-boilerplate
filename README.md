# Nuxt Boilerplate

A ready to use Nuxt 4 boilerplate

## Quick setup (TLDR;)

```bash
git clone https://github.com/forgeon-apps/nuxt-boilerplate.git
cd nuxt-boilerplate
pnpm install
pnpm run dev
```

## Setup

### Prerequisites:

- [pnpm](https://pnpm.io/)
- [mkcert](https://github.com/FiloSottile/mkcert) (Optional localhost HTTPS)

### Clone repo

```bash
git clone https://github.com/forgeon-apps/nuxt-boilerplate.git
cd nuxt-boilerplate
```

### Install dependencies:

```bash
pnpm install
```

### Optional: `.env`

```ini
VITE_BASE_URL="https://localhost:3000/"
```

### Optional: Generate certificate for HTTPS for localhost

```bash
# mkdir certs
cd certs
mkcert localhost
```

## Start local server

### Start development server

```bash
# HTTP
pnpm run dev
# HTTPS
pnpm run dev-https
```

### Start production build server (HTTP)

```bash
# HTTP
pnpm run build;pnpm run preview
# HTTPS
pnpm run build;pnpm run preview-https
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.
