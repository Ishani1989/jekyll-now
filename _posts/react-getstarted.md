---
layout: post
title: Creating your first application in React!
---

## It's time to React

First things first, lets make things clear. 

#### What is React ?

React is nothing but Javascript. If you know Javscript, React should come pretty easily to you.
React is nothing but a framework that allows you to write declarative code with much less hassle for each simple step.
It supports unidirectional data flow unlike Angular or Ember where data is in sync throught the app no matter where it has been updated from.
#### Understand how React works :

##### React uses JSX:

###### What is JSX ?

JSX is nothing but adding XML like structure to javascript. JSX allows React components to return an HTML elemnt instead of just a single value.
JSX allows to embed HTML tags and javascript notations all in one place.

##### React returns UI instead of just elements.

Each c;lass in React will display something on the DOM, only when its `render` method is called. Hence, each React class must have a render method.
Each render method should return some UI in order to be shown on the screen. Only a single elements may be returned, hence it is necessary to wrap all elements within a single HTML tag.

React lays out the foundation for 2 basic concepts :

1. **State**
2. **Components**

##### State : 

The state variable in React is used to store data which on change will be responsible to re-remder the screen automatically.
Whenever the state for an application is changed, React will re render your application and you do not need to manually refresh it.

##### Components :

Components are the building blocks that is used to compose your application. Each functionality in React should be broken down into components.
The connection between components is maintained by values that we pass to child components called 'props'.

##### JSX and ES6:

Most React componenets are developed using JSX instead of plain javascript. Now, what is JSX ?
JSX is a programmic language that uses XML like formatting with javascript. Using JSX you can directly embed HTML tags within your javascript methods.
It makes using React a lot more elegant and faster.

React uses ES6 syntax for all its methods. React is declarative in nature. Using arrow functions is the most common in React.

```
this.nums.forEach((v) => {
    if (v % 5 === 0)
        this.fives.push(v)
})
```

##### `render` and `return` are absolutely mandatory in React:

Each componenet can be composed either as a class that extends `React.component` or a functional component that has nothing but a `render` method.

All components **must** have a `render` method if they ARE supposed to be included within the DOM.
All `render` methods **must** have a return statement that will return not a single value but some UI to the DOM.

```
class FirstExample extends Component{

render {
    return (<div>Hello World</div>)
}

```
##### Nesting of components :

Its best practice to break all functionalities into separate components in React.
 In order to do so, simply in a new file define a new class as
 
 ```
class ComponentName extends Component{
    
    render{
        return ('some UI')
        }
    }

export default ComponentName
```

To include this in your parent component :

```
import ComponentName from './path'
```

Then use it simply like a self ending HTML tag in your render method.

```
render {
    return(
        <ComponentName/>
        })
}
```

##### Passing data within components :

**props** is the keyword that will help you here. All data that is passed within components using this.props.
Here, `this` is used to denote the current components context.

Pass the props to the child component like this :

```
const data= "Welcome to React"
<ComponentName data = {this.data}/>

```
Within the child component we can access the value stored in data like this :

```
render{
    return(
        <div>{this.props.data}</div>
    )}
```
This will output 'Welcome to React' in the DOM.

##### Routing in React :

React provides built-in components for most of the common functions needed by developers.
 The `Route` component along with the `Link` package can make it super easy to route to a particular URL.
 
 Many other router packages are available such as
 
 * hashRouter
 * browserouter
 * withRouter
 
 `withRouter` is used to automatically navigate to a path from within a method in React.
 You just need to enclose the calling component as
 
 `export default withRouter([component name])`

##### Steps to start a react application:

1. Download and install npm. This is the basic package manager you will need to install all dependencies.
2. Once done install create-react-app globally to scaffold your initial react application.

    `npm install -g create-react-app`

3. Create a new folder and navigate to it on your terminal and run the command

    `create-react-app {Your project name}`
4. Run `npm install` to install all React dependencies mentioned in the package.json file.
5. Once installed run the command `npm start`. React automatically runs scripts to open a demo app at localhost:3000.



