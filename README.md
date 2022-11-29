# Docker Resources

## Prerequisites

- Download extension and **Prettier - Code formatter** in your VSCode.
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

- **(Optional):** Install dependencies.

```bash
$ pnpm i
```

## Run resources

- Navigate to specific resource.

```bash
$ cd <resource>
```

#### Assuming you're already in the resource directory.

- Run/Start the resource.

```bash
$ docker compose up -d
```

- Stop the resource.

```bash
$ docker compose stop
```

- Shutdown the resource.

```bash
$ docker compose down
```
