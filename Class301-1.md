# This is my journal 7/16/2022

## What I have learned today

- Today I read about components and props.

> “Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another. (//itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0)

- Data with props pass through a one way flow from parent to child.

- Props data is read only data

- Firstly, define an attribute and its value(data).Then pass it to child component(s) by using Props.Finally, render the Props Data.

Example: class ParentComponent extends Component
 <!-- {  
  render() {
    return (
      <h1>
        I'm the parent component.
        <ChildComponent />
      </h1>
    );
  }
} -->

- Child component

<!-- const ChildComponent = () => {  
  return <p>I'm the 1st child!</p>; 
}; -->

> Component-based architecture focuses on the decomposition of the design into individual functional or logical components that represent well-defined communication interfaces containing methods, events, and properties. It provides a higher level of abstraction and divides the problem into sub-problems, each associated with component partitions. (www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

- The primary use of components is for reusability.

- A component is a modular, replaceable and reusable set of well defined functionality.

- There are three views of components, object-oriented, conventional view, process related view.

- 