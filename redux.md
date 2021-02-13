# Redux

## Review, Research, and Discussion

### What are the advantages of storing tokens in “Cookies” vs “Local Storage”
**Cookies are better to used in handling the user data especially these data are secret, so it will be hard to get XSS attack.**

### Explain 3rd party cookies.
**It is an information that stored in the client computer of the specified site and let be used easily to track the user during their access to the web routes.**

### How do pixel tags work?
**It is useful to track the user behavior and conversions.**

## Document the following Vocabulary Terms
- **_cookies_** is a user information where is stored in the client computer.
- **_authorization_** where the user is authorized to access any route.
- **_access control_** means controling the access of the user based on the user's role.
- **_conditional rendering_** is rendering a piece of data based on the user request.

## Preparation Materials
***Redux is a javascript library wher is used in the front-end part, and it could be installed from the node package manager (npm) and therefore you coulc use the mothod called createStore where is storing and handling the data of the webpage from any action that is going to be taken from the user.Then, getState() will be responsible for the getting an updating the data, dispatch() will check and store the type of action that the user made, and subscribe() will push any changes made to the state variable.***