# AWS Web Server Automator

## Setup
You'll need to provide your AWS credentials. This can be done by having the
local environment variables defined in `.env` or in your shell:

```shell
AWS_ACCESS_KEY_ID=YOUR_KEY
AWS_SECRET_ACCESS_KEY=YOUR_SECRET_KEY
```

## Creating the Stack
```shell
docker-compose run --rm aws create
```

Should you wish to override the `STACK_NAME`, you can:

```shell
docker-compose run --rm aws create -e STACK_NAME=awesome-stack
```

## Deleting the Stack
```shell
docker-compose run --rm aws delete
```
