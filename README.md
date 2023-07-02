# Component Life Cycle

- Mounting Phase
  - constructor()
  - render()
  - componentDidMount()
- Updating Phase
  - render()
- Unmounting phase
  - componentWillUnmount()
- Behind the scenes
  - Virtual DOM

Every React Component goes through three phases throughout its lifetime:

- Mounting Phase
- Updating Phase
- Unmounting phase

## Mounting Phase
In this phase, the instance of a component is created and inserted into the DOM.

### Methods
We mainly use the three methods. The three methods are called in the given order:

- constructor()
- render()
- componentDidMount()
  
### constructor()
The constructor() method is used to set up the initial state and class variables.

We must call the super(props) method before any other statement. Calling super(props) makes sure that constructor() of the React.Component gets called and initializes the instance.

Initialising State through props
  - this.state={key:value}

### render()
The render() method is used to return the JSX that is displayed in the UI.

### componentDidMount()
The componentDidMount() method is used to run statements that require that the component is already placed in the DOM.

Example: set timers, initiate API calls, etc.

## Updating Phase
In this phase, the component is updated whenever there is a change in the component's state.

### render()
The render() method is called whenever there is a change in the component's state.

## Unmounting Phase
In this phase, the component instance is removed from the DOM.

### componentWillUnmount()
The componentWillUnmount() method is used to cleanup activities performed.

Example: clearing timers, cancelling API calls, etc.
