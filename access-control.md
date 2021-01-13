# Access Control (ACL)

## Review, Research, and Discussion

### When is Basic Authorization used vs. Bearer Authorization?
**Basic Authorization used when the user logged in to generate an access token from the request header, however, the bearer authorization will get the user permission after logged in or signed up for accessing other routes.**

### What does the JSON Web Token package do?
**It is a package that used in order to generate a token that sould be useful for the user to acces other routes.**

### What considerations should we make when creating and storing a SECRET?
**The secret variable should be something unique and hard to guess. Also, it should be inside a hidden file such as '.env' file**


## Document the following Vocabulary Terms

- **_encryption_** it is a process to encode any secret string, so it will hard for any hackers to decode it again and turn it back to a plain text.

- **_token_** it is a set of characters that generated once the user logged in or sign up to use for authenticate the user over all of the website routes.

- **_bearer_** it is a middleware that used to verify the user in order to get a permission to access all the website routes.

- **_secret_** it is a string that store safely, securely and uniquely so it will be hard to find or even guess what it is.

- **_JSON Web Toke_** is a npm package that useful to sign a token and verify it to check the user and give her/him a permission to access all the routes.