# Redux - Asynchronous Actions

## Review, Research, and Discussion
### How granular should your reducers be?
**The reducer will be helpful that each set of actions have their own reducer function.**

### Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
**Yes, definitely they will fire all of the reducers that shares the same name of the action.**

### Name a strategy for preventing the above
**It has a different action type for each other.**

## Document the following Vocabulary Terms
- **_store_** is a file that has the initial state and its reducer function where based on the action, these actions will apply a certain changes and return it to its component.
- **_combined reducers_** is an option to combined all of the reducers in one store that could be shared among all of the components.

## Preview
**Asynchronous Actions - Where is getting its initial data from external API. This initail state will have a three keys/values, these are a loading boolean where to show a load snippet while it is getting the data from the API, the second one will be the data that is fetched from the API, and finally the error where is sent based on the condition of the fetching API. Of course, the asynchronous will have also the same with the synchronous action such as reducer and the action functions.**