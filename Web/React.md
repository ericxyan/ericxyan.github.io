# React.js Note
## Tools
- Chrome plugin: react-devtools
- NPM: create-react-typescript

## Tips
- Use function component as much as you can
- Child component cannot access to siblings' properties directly
- spread operator: ``...``
- 

## Redux
### 3 Principles
1. All states in one immutable store 
2. Actions trigger changes
3. Reducers update state 

#### Core Principles
- 1 Store, multiple Reducers
- All Reducers are called on each dispatch


### Reducer
````
(state, action) => state
````
#### Forbidden in Reducers
- Mutate args
- Perform side effects
- Call non-pure functions
 
## React-Redux

### Three Principles
#### Single source for truth
The state of whole app is stored in a single store
#### State is read-only
The only way to change a state is to emit an action
#### Changes are made with pure functions
reducers: specify how the state tree is transformed by actions



### Provider
Attaches app to store
````
<Provider store={this.props.store}>
	<App />
</Provider>
````

### Connect
Creates container components; Wraps components so it's connected ot the Store
````
export default connect(
	mapStateToProps,
	mapDispatchToProps
)(AuthorPage);
````
- ``mapStateToProps``: what states will be exposed as props
- ``mapDispatchToProps``:  what actions will be exposed as props, 3 ways:

 
