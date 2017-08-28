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

1. State
2. Components

##### State : 

The state variable in React is used to store data which on change will be responsible to re-remder the screen automatically.
Whenever the state for an application is changed, React will re render your application and you do not need to manually refresh it.

##### Components :

Components are the building blocks that is used to compose your application. Each functionality in React should be broken down into components.
The connection between components is maintained by values that we pass to child components called 'props'.

##### Steps to start a react application:

1. Download and install npm. This is the basic package manager you will need to install all dependencies.
2. Once done install create-react-app globally to scaffold your initial react application.

    `npm install -g create-react-app`

3. Create a new folder and navigate to it on your terminal and run the command

    `create-react-app {Your project name}`
4. Run `npm install` to install all React dependencies mentioned in the package.json file.
5. Once installed run the command `npm start`. React automatically runs scripts to open a demo app at localhost:3000.



