# Character Queries

This directory contains GraphQL queries to fetch character information from the Rick and Morty API.

## Files

- `character-id-1.graphql`: Query to fetch character with ID 1 (Rick Sanchez)
- `character-id-1-output.json`: Expected output for character ID 1
- `character-id-2.graphql`: Query to fetch character with ID 2 (Morty Smith)
- `character-id-2-output.json`: Expected output for character ID 2
- `character-id-3.graphql`: Query to fetch character with ID 3 (Summer Smith)
- `character-id-3-output.json`: Expected output for character ID 3
- `character-id-4.graphql`: Query to fetch character with ID 4 (Beth Smith)
- `character-id-4-output.json`: Expected output for character ID 4

## Query Details

Each query fetches the following fields for a character:
- `id`: The id of the character
- `name`: The name of the character
- `status`: The status of the character (Alive/Dead/unknown)
- `species`: The species of the character
- `type`: The type or subspecies of the character
- `gender`: The gender of the character

## How to Use

You can execute these queries against the Rick and Morty GraphQL API endpoint:
`https://rickandmortyapi.com/graphql`

Example using curl:
```bash
curl -X POST \
  -H "Content-Type: application/json" \
  -d @character-id-1.graphql \
  https://rickandmortyapi.com/graphql
```
