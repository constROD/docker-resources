# Docker Resources

## Available resources

- postgres

## Prerequisites

- Download extension **ESLint** and **Prettier - Code formatter** in your VSCode.
- Install **node** >= 16.13.0
- Install **pnpm** >= 7.17.0

- **(Required for MacOSX):** Run this to give permission husky to run pre-commit hook.

```bash
$ chmod ug+x .husky/*
$ chmod ug+x .git/hooks/*
```

- **(Optional):** Do this if you are using **nvm**.

```bash
$ nvm use or nvm use 16.13.0
```

- Install dependencies.

```bash
$ pnpm i
```

- Build container.

```bash
$ docker compose -f ./<resource_name>/docker-compose.yaml or pnpm docker:<resource_name> build # Build with cache
```

```bash
$ docker compose -f ./<resource_name>/docker-compose.yaml build --no-cache or pnpm docker:<resource_name> build --no-cache # Build with no cache
```

- Run container.

```bash
$ docker compose -f ./<resource_name>/docker-compose.yaml up or pnpm docker:<resource_name> up # Run in foreground
```

```bash
$ docker compose -f ./<resource_name>/docker-compose.yaml up -d or pnpm docker:<resource_name> up -d # Run in background
```

- Shutdown container.

```bash
$ docker compose -f ./<resource_name>/docker-compose.yaml down or pnpm docker:<resource_name> down # Remove without volumes
```

```bash
$ docker compose -f ./<resource_name>/docker-compose.yaml down -v or pnpm docker:<resource_name> down -v # Remove with volumes
```

**Access the container:**

```bash
$ docker exec -it <container_name> bash
```

```bash
$ docker logs <container_name>
```
