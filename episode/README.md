# Episode Queries

This directory contains GraphQL queries to fetch episode information from the Rick and Morty API.

## Files

- `episode-1.graphql`: Query to fetch episode with ID 1 (Pilot)
- `episode-1-output.json`: Expected output for episode ID 1
- `episode-2.graphql`: Query to fetch episode with ID 2 (Lawnmower Dog)
- `episode-2-output.json`: Expected output for episode ID 2
- `episode-3.graphql`: Query to fetch episode with ID 3 (Anatomy Park)
- `episode-3-output.json`: Expected output for episode ID 3
- `episode-4.graphql`: Query to fetch episode with ID 4 (M. Night Shaym-Aliens!)
- `episode-4-output.json`: Expected output for episode ID 4

## Query Details

Each query fetches the following fields for an episode:
- `id`: The id of the episode
- `name`: The name of the episode
- `air_date`: The air date of the episode
- `episode`: The code of the episode (e.g., S01E01)

## How to Use

You can execute these queries against the Rick and Morty GraphQL API endpoint:
`https://rickandmortyapi.com/graphql`

Example using curl:
```bash
curl -X POST \
  -H "Content-Type: application/json" \
  -d @episode-1.graphql \
  https://rickandmortyapi.com/graphql
```
