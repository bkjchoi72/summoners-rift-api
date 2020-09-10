# summoners-rift-api
This service allows you to add/get/update/remove champions via RESTful API.

## Endpoints
* POST /champion
    * Create and store a champion
    * Return the ID of the champion that was created
* GET /champion/id
    * Get details about a champion by ID
* DELETE /champion/id
    * Delete a champion by id
* GET /champion?type=
    * Get all champions of a given type
* GET /champion?role=
    * Get all champions of a given role
## Sample payload
* {“name”: “zed”, “type”: “assassin”, “roles”:[“middle”]}
* {“name”: “ashe”, “type”: “marksman”, “roles”:[“adc”, “support”]}
