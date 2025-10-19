# 2. Write a Query to Get a Specific Episode by ID


## Objective
Learners will write a GraphQL query to fetch the details of a specific episode using its ID.


## Endpoint
Use the provided GraphQL endpoint (e.g., Rick and Morty GraphQL API). The task uses the `episode(id: ID!)` field.


## Instructions
1. Write a GraphQL query using the `episode(id: ID!)` field to retrieve details of an episode.
2. Use IDs `1`, `2`, `3`, and `4` — one query per file.
3. Include the following fields: `id`, `name`, `air_date`, and `episode`.


## Files included
- `episode-id-1.graphql`
- `episode-id-1-output.json`
- `episode-id-2.graphql`
- `episode-id-2-output.json`
- `episode-id-3.graphql`
- `episode-id-3-output.json`
- `episode-id-4.graphql`
- `episode-id-4-output.json`


## How to run
1. Open any `.graphql` file in your GraphQL client (Insomnia, Postman, GraphiQL, or curl).
2. Send the query to the endpoint.
3. Compare the returned JSON response with the corresponding `-output.json` file.