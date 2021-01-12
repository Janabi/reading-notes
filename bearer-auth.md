# Bearer Authorization

## Review, Research, and Discussion

### Write the following steps in the correct order:
- Register your application to get a client_id and client_secret.
- Ask the client if they want to sign in via a third party.
- Redirect to a third party authentication endpoint.
- Make a request to a third-party API endpoint.
- Receive authorization code.
- Make a request to the access token endpoint.
- Receive access token.

### What can you do with an authorization code?
**It will allow the website to access the user info and safe it in the database.**

### What can you do with an access token?
**It is useful as a key to get the permission or authorization to take the user info from another website API.**

### What’s a benefit of using OAuth instead of your own basic authentication?
**Its benefit for accessing the other web server.**


## Document the following Vocabulary Terms

- **_Client ID_** it is one of the parameter of getting the access token, and the developer can get it from any website that would providing the feature of accessing some of their user info.

- **_Client Secret_** it is one of the parameter of getting the access token, and the developer can get it from any website that would providing the feature of accessing some of their user info.

- **_Authentication Endpoint_** it is secure way to make a certain authorized server can connect to their server.

- **_Access Token Endpoint_** it is a server request to get the access token in order to be authorized to get a data from another server.

- **_API Endpoint_** it is a queries in order to have a comunication between the user and the API.

- **_Authorization Code_** a code that the user send it to the authorization API to get an access token.

- **_Access Token_** the server is authorized to get a selected user info from other server.