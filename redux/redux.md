<h1 style="font-family: Roboto" align="center">
REDUX CHEAT SHEET
</h1>

<h3 style="font-family: Roboto">
Creating a Store
</h3>

```jsx
import { createStore } from 'redux'

// Reducer
function counter (state = { value: 0 }, action) {
	switch (action.type) {
		case 'INCREMENT':
			return { value: state.value + 1 }
		case 'DECREMENT':
			return { value: state.value - 1 }
		default:
			return state
	}
}

let store = createStore(counter)
// Optional - you can pass `initialState` as a second arg
let store = createStore(counter, { value: 0 })
```

<h3 style="font-family: Roboto">
Using a Store 
</h3>

```jsx
let store = createStore(counter)

// Dispatches an action; this changes the state
store.dispatch({ type: 'INCREMENT' })
store.dispatch({ type: 'DECREMENT' })

// Gets the current state
store.getState()

// Listens for changes
store.subscribe(() => { ... })
```

<h3 style="font-family: Roboto">
Provider 
</h3>

```jsx
import { Provider } from 'react-redux'

React.render(
  <Provider store={store}>
    <App />
  </Provider>)
```

<h3 style="font-family: Roboto">
Mapping State 
</h3>

```jsx
import { connect } from 'react-redux'

// A functional React component
function App ({ message, onMessageClick }) {
  return (
    <div onClick={() => onMessageClick('hello')}>
      {message}
    </div>
  )
} 

// Maps `state` to `props`:
// These will be added as props to the component.
function mapState (state) {
  return { message: state.message }
}

// Maps `dispatch` to `props`:
function mapDispatch (dispatch) {
  return {
    onMessageClick (message) {
      dispatch({ type: 'click', message })
    }
  }
}

// Connect them:
export default connect(mapState, mapDispatch)(App)
```

<h3 style="font-family: Roboto">
Shorthand 
</h3>

```jsx
export default connect(
  (state) => ({
    message: state.message
  }),
  (dispatch) => ({
    onMessageClick: (message) => {
      dispatch({ type: 'click', message })
    }
  })
)(App) 
```

<h3 style="font-family: Roboto">
Combining Reducers 
</h3>

```jsx
const reducer = combineReducers({
  counter, user, store
}) 
```

