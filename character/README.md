# alx-graphql-0x00 — character

This document contains the `README.md`, four GraphQL query files and their expected output JSON files for the **"0. Write a Query to Get a Specific Character by ID"** task.

---

## File: README.md

```md
# 0. Write a Query to Get a Specific Character by ID

## Objective
Learners will write a GraphQL query to retrieve a specific character’s information using their ID.

## Endpoint
Use the GraphQL endpoint provided by the course (e.g. a Rick and Morty GraphQL endpoint). The task expects queries that use the `character(id: ID!)` field.

## Instructions
1. Write a GraphQL query using the `character(id: ID!)` field to fetch the details of a character.
2. Use IDs `1`, `2`, `3`, and `4` — one query per file.
3. Include the following fields in your query: `id`, `name`, `status`, `species`, `type`, `gender`.

## Files included
- `character-id-1.graphql`
- `character-id-1-output.json`
- `character-id-2.graphql`
- `character-id-2-output.json`
- `character-id-3.graphql`
- `character-id-3-output.json`
- `character-id-4.graphql`
- `character-id-4-output.json`

## How to run
1. Point your GraphQL client (Insomnia, GraphiQL, Postman, curl) to the provided endpoint.
2. Open the appropriate `.graphql` file and send the query.
3. Compare the response with the corresponding `-output.json` file.

## Notes
- Some GraphQL servers accept IDs as integers (e.g. `character(id: 1)`) and some require string IDs (e.g. `character(id: "1")`). Use whichever form the endpoint requires. The example queries here use numeric IDs.
```

---

## File: character-id-1.graphql

```graphql
# Query to fetch character with id 1
query GetCharacterById {
  character(id: 1) {
    id
    name
    status
    species
    type
    gender
  }
}
```

## File: character-id-1-output.json

```json
{
  "data": {
    "character": {
      "id": "1",
      "name": "Rick Sanchez",
      "status": "Alive",
      "species": "Human",
      "type": "",
      "gender": "Male"
    }
  }
}
```

---

## File: character-id-2.graphql

```graphql
# Query to fetch character with id 2
query GetCharacterById {
  character(id: 2) {
    id
    name
    status
    species
    type
    gender
  }
}
```

## File: character-id-2-output.json

```json
{
  "data": {
    "character": {
      "id": "2",
      "name": "Morty Smith",
      "status": "Alive",
      "species": "Human",
      "type": "",
      "gender": "Male"
    }
  }
}
```

---

## File: character-id-3.graphql

```graphql
# Query to fetch character with id 3
query GetCharacterById {
  character(id: 3) {
    id
    name
    status
    species
    type
    gender
  }
}
```

## File: character-id-3-output.json

```json
{
  "data": {
    "character": {
      "id": "3",
      "name": "Summer Smith",
      "status": "Alive",
      "species": "Human",
      "type": "",
      "gender": "Female"
    }
  }
}
```

---

## File: character-id-4.graphql

```graphql
# Query to fetch character with id 4
query GetCharacterById {
  character(id: 4) {
    id
    name
    status
    species
    type
    gender
  }
}
```

## File: character-id-4-output.json

```json
{
  "data": {
    "character": {
      "id": "4",
      "name": "Beth Smith",
      "status": "Alive",
      "species": "Human",
      "type": "",
      "gender": "Female"
    }
  }
}
```

---

> **Reminder:** If your endpoint requires string IDs, change `character(id: 1)` to `character(id: "1")` in each `.graphql` file.
