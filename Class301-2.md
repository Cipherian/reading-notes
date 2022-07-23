# This is my journal 7/20/2022

- React lets you define components as classes or functions.

> These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.

- Mounting: when an instance of a component is being created and inserted into the dom, it happens during the mounting phase. (Constructor, static, getDerivedStateFromProps, componentDidMount, and UNSAFE_componentWillMount all occur during mounting.)

- When a componenent is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order.

- Unmounting: The final phase of a lifecycle when a component is being removed from the DOM.

- The constructor for a React component is called before it is mounted.

- If the component is a subclass you should call super(props), or the props will be undefined.

> Example: class FishTableRow extends React.Component {
  constructor() {
    super(props);
    this.state = {
      property:here
    }
  }
};

- Avoid using this.setState() in the constructor because it can lead to side effects.

- render is the only required mehtod in a class component. IT will examine this.props and this.state when called. The render function should not modify the component state because that would cause problems when it has to rerender and should not interact with the browswer.

> componentDidMount() This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().

setState() can be called here, but it should be used sparingly, because it will cause a rerender, which can lead to perfomance issues.

Here we use componentDidMount() to connect to the YouTube API and get videos when the components is rendered.

> EX: componentDidMount() {

console.log(‘got videos’);

this.getVideos(‘cats’);

}

getVideos(query) {

var options = {

key: this.props.YOUTUBE_API_KEY,

query: query

};

- Source: (medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

- React vs State

- Props are arguments to a function. You pass in the props you want to give to a function.

- State is something inside of a component. It is handled only inside of a component. When you change state, it rerenders the webpage.

- State is there for when you need to rerender your application when the user do something.

