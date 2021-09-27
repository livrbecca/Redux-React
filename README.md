# Redux-React Crash Course

Redux a library used used for **state management**.
All application state is centralized is saved inside a 'store', which lets the data be in-sync with each other.
Makes data flow transparent and predictable.

# The store

-A JS object, accessible by all parts of the UI.
-Can contain arrays, objects, booleans, etc.
-Not for dirently modifying or mutating state. The store is an immutable object, update it using a fucntion and spread operator.

# Reducer

A reducer is a function that takes the current instance of the store, and returns the updated store

```
function reducer(store, action){
    const updated = {...store};
}

```
