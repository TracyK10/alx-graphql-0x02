# Character Queries

This directory contains GraphQL queries to fetch character information from the Rick and Morty API.

## Files

### Single Character Queries
- `character-id-1.graphql`: Query to fetch character with ID 1 (Rick Sanchez)
- `character-id-1-output.json`: Expected output for character ID 1
- `character-id-2.graphql`: Query to fetch character with ID 2 (Morty Smith)
- `character-id-2-output.json`: Expected output for character ID 2
- `character-id-3.graphql`: Query to fetch character with ID 3 (Summer Smith)
- `character-id-3-output.json`: Expected output for character ID 3
- `character-id-4.graphql`: Query to fetch character with ID 4 (Beth Smith)
- `character-id-4-output.json`: Expected output for character ID 4

### Paginated Character Queries
- `characters-page-1.graphql`: Query to fetch first page of characters (IDs 1-20)
- `characters-page-1-output.json`: Expected output for page 1
- `characters-page-2.graphql`: Query to fetch second page of characters (IDs 21-40)
- `characters-page-2-output.json`: Expected output for page 2
- `characters-page-3.graphql`: Query to fetch third page of characters (IDs 41-60)
- `characters-page-3-output.json`: Expected output for page 3
- `characters-page-4.graphql`: Query to fetch fourth page of characters (IDs 61-80)
- `characters-page-4-output.json`: Expected output for page 4

## Query Details

### Single Character Queries
Each query fetches the following fields for a specific character:
- `id`: The id of the character
- `name`: The name of the character
- `status`: The status of the character (Alive/Dead/unknown)
- `species`: The species of the character
- `type`: The type or subspecies of the character
- `gender`: The gender of the character

### Paginated Character Queries
Each paginated query fetches the following fields for each character in the page:
- `id`: The id of the character
- `name`: The name of the character
- `status`: The status of the character (Alive/Dead/unknown)
- `image`: URL to the character's image

## How to Use

You can execute these queries against the Rick and Morty GraphQL API endpoint:
`https://rickandmortyapi.com/graphql`

Example using curl for a single character query:
```bash
curl -X POST \
  -H "Content-Type: application/json" \
  -d @character-id-1.graphql \
  https://rickandmortyapi.com/graphql
```

Example using curl for a paginated query:
```bash
curl -X POST \
  -H "Content-Type: application/json" \
  -d @characters-page-1.graphql \
  https://rickandmortyapi.com/graphql
```
