# nexus-prisma

`nexus-prisma` is a POC. I was curious to see how straightforward creating an API with [Nexus](https://nexus.js.org/docs/getting-started) and [Prisma](https://www.prisma.io/) would be.

## Setup

Install all the dependencies:

```sh
yarn

# npm i
```

Since a Postgres database is needed for this app. I would recommend running a Postgres server using Docker:

```sh
docker run --detach --publish 5432:5432 -e POSTGRES_PASSWORD=docker --name postgres
```

Run the migrations:

```sh
npx prisma migrate up --experimental
```

Run the server:

```sh
yarn dev

# npm run dev
```

## Usage

Now you're able to work with the API through the GraphQL Playground at [localhost:4000](http://localhost:4000)

## Acknowledgment

This project was created by following the [Nexus' official tutorial](https://nexusjs.org/getting-started/tutorial).

## License

[MIT](https://choosealicense.com/licenses/mit/)
