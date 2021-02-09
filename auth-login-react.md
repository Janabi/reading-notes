# <Login /> and <Auth />

## Review, Research, and Discussion
### Why is the Context API useful?
**It could be used as aparent of the general component within the app and once you would like to change something it will automatically change to the other components.**

### Can a component outside of a provider get its context?
**Yes, any components can access the provider even if it is outside.**

### What are some common use cases for using the Context API?
**Dark or light mode is a common use case for the context API.**

### Describe “Context Hell”
**it is a method that commonly used to wrappe up the whole components into a single one.**

## Document the following Vocabulary Terms

- **_global state_**  a state variable where it passed through the whole children of the parent's component.
- **_global context_** is a hook method that would used to passed a certain variable or functionality to the whole ap components.
- **_provider_** where it will provide the creation of the context and wrape with it the variable that would like to transfer.
- **_consumer_** where it is going to consume the context within the general or parent component

## Preview
***Now, we will use the role-based access control (RBAC) to authorize the user to enter a certain routes based on the user's role on this website app. This will make the data more secure and maintainable. This could be accomplish by using the react cookies that would check if there is a logged in user or not.***