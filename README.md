# Redux-React Crash Course

Redux a library used used for **state management**.
All application state is centralized is saved inside a 'store', which lets the data be in-sync with each other.
Makes data flow transparent and predictable.

# The store

-A JS object, accessible by all parts of the UI.

-Can contain arrays, objects, booleans, etc.

-Not for dirently modifying or mutating state. The store is an immutable object, update it using a fucntion and spread operator.

# Reducer

A reducer is a function that takes the current instance of the store, and returns the updated store.

Can have 1 or more. Each reducer is responsible for updating a slice of the store. Think of them like event handlers

```
function reducer(store, action){
    const updated = {...store};
}

```

**How the reducer knows what properties to update:** identified from a building block called *action*

# Action
Plain JS object that describes what just happened. Think of them as 'events;

- examples: user logged in, user logged out, added item to cart, removed item from cartm ect.

- Action is passed to a reducer as the second parameter

- Based on the type of the action, the reducer will know what properties to update
