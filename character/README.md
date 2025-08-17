# GraphQL Characters Queries

This project contains GraphQL queries and their outputs for fetching characters from the [Rick and Morty GraphQL API](https://rickandmortyapi.com/graphql).

## Files

- `characters-page-1.graphql` – Query for page 1
- `characters-page-1-output.json` – Results for page 1
- `characters-page-2.graphql` – Query for page 2
- `characters-page-2-output.json` – Results for page 2
- `characters-page-3.graphql` – Query for page 3
- `characters-page-3-output.json` – Results for page 3
- `characters-page-4.graphql` – Query for page 4
- `characters-page-4-output.json` – Results for page 4

## Usage

You can run the queries against the API using any GraphQL client (e.g., [Apollo Studio](https://studio.apollographql.com/sandbox) or `curl`).

Example with `curl`:

```bash
curl -X POST https://rickandmortyapi.com/graphql \
  -H "Content-Type: application/json" \
  -d '{"query":"{ characters(page: 1) { results { id name status image } } }"}'
