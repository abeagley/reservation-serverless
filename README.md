# Reservation Serverless Service

### What is this?

An example of a serverless RESTful and GraphQL api. For a sample UI consuming these services checkout: 
[Sample UI](https://github.com/abeagley/reservation-ui).

<a href="http://www.youtube.com/watch?feature=player_embedded&v=Vc3hcwFscME
" target="_blank"><img src="http://img.youtube.com/vi/Vc3hcwFscME/0.jpg" 
alt="Intro Video" width="240" height="180" border="10" /></a>

---

### Getting Started

PRE) You need to have the AWS CLI installed and configured with your credentials. This
serverless application will take care of creating the Dynamo table it uses for persistance.

1) `$ npm install -g serverless`
2) `$ npm install`
3) `$ npm run deploy` 

This will give you AWS lambda URL's and create a Dynamo table

##### Offline:

4) `$ npm start`

Runs an offline version of lambdas for local development

----------

That's it. The application is up and running and you can use either GraphQL or the RESTful 
endpoints to interact with the service.

----------

### Example Endpoints

```
# GraphQL
POST - https://ja8ibi4phg.execute-api.us-west-2.amazonaws.com/api/graphql

# REST
GET  - https://ja8ibi4phg.execute-api.us-west-2.amazonaws.com/api/reservations
GET  - https://ja8ibi4phg.execute-api.us-west-2.amazonaws.com/api/reservations/{id}
POST - https://ja8ibi4phg.execute-api.us-west-2.amazonaws.com/api/reservations
```

##### Postman:

I've included a Postman collection for those who utilize it:

`./reservations.postman_collection.json`
