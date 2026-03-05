# API Testing Example – JSONPlaceholder

This folder contains an example Postman collection used to test a public REST API.

## Endpoints Tested

- GET /posts/1 → single post
- GET /posts → all posts
- GET /posts/999999 → non-existing post

## Automated Tests Included

- Status code verification
- Response structure verification
- Error response verification

Open `jsonplaceholder-api-tests.postman_collection.json` in Postman to run these tests.