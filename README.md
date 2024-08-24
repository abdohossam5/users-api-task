## About

Sample API for interview task

## Task
- Add new endpoint to get all users
- The endpoint should accept optional parameters to allow querying by specific skill

sample request
```shell
curl -X GET http://localhost:3000/users/all?skill=java
```
sample response
```json
{
  "users": [{
      "id": 310946254456,
      "name": "John Smith",
      "email": "john.smith@example.com",
      "created": "2024-03-22T05:20:55.079Z",
      "skills": [
        {
          "id": 1,
          "name": "Java",
          "level": "Intermediate"
        },
        {
          "id": 2,
          "name": "Spring Boot",
          "level": "Intermediate"
        }
      ]
  }]
}
```


## Available Scripts

### `npm run dev`

Run the server in development mode.

### `npm test`

Run all unit-tests with hot-reloading.

### `npm test -- --testFile="name of test file" (i.e. --testFile=Users).`

Run a single unit-test.

### `npm run test:no-reloading`

Run all unit-tests without hot-reloading.

### `npm run lint`

Check for linting errors.

### `npm run build`

Build the project for production.

### `npm start`

Run the production build (Must be built first).

### `npm start -- --env="name of env file" (default is production).`

Run production build with a different env file.


## Additional Notes

- If `npm run dev` gives you issues with bcrypt on MacOS you may need to run: `npm rebuild bcrypt --build-from-source`. 
