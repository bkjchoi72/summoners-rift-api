# summoners-rift-api
This service allows you to add/get/update/remove champions via REST API.

## Endpoints
- POST /champion
    - Create and store a champion
    - Return the ID of the champion that was created
    - payload example: {“name”: “ashe”, “type”: “marksman”, “roles”:[“adc”, “support”]}
    - response example: {"id": 0, "name": "ashe", "type": "marksman", "roles":["adc", "support"]}
- PUT /champion/id
    - Create a new or update existing champion by ID
- GET /champion/id
    - Get details about a champion by ID
    - response example: {“name”: “ashe”, “type”: “marksman”, “roles”:[“adc”, “support”]}
- PUT /champion/id
    - Creates a new or updates existing champion by ID
- DELETE /champion/id
    - Delete a champion by id
    - Return an empty response
- GET /champion?type=
    - Get all champions of a given type
- GET /champion?role=
    - Get all champions of a given role
- GET /random-team
    - Return a team of 5 champions ({“jungle”:<champ 1 info>, “adc”:<champ 2 info>...})that fill all the required roles of Summoners Rift
## Sample payload
- {“name”: “zed”, “type”: “assassin”, “roles”:[“middle”]}
- {“name”: “ashe”, “type”: “marksman”, “roles”:[“adc”, “support”]}
