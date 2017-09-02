The following guide will take you towards building your first project in React. Here, we will be creating a simple puzzle game using React.

Steps :

1. Create a directory in your local machine and browse to the directory in your terminal.
2. Run the command ```create-react-app MyPuzzleGame```
3. This will download all necessary files to your system.

The command will create the following structure.

We need to make modifications to the src folder in order to implement our game.

####Breaking down into components:

We can think of our game in terms of smaller components that we can combine to create our app.

1. app.js - main file
2. grid.js - the grid for the puzzle
3. pic.js - component to hold individual pic for puzzle.

#####app.js

```
import React, { Component } from 'react';
import logo from './logo.svg';
import './App.css';

class App extends Component {
  render() {
    return (
      <div className="App">
        <div className="App-header">
          <img src={logo} className="App-logo" alt="logo" />
          <h2>Welcome to React</h2>
        </div>
        <p className="App-intro">
          To get started, edit <code>src/App.js</code> and save to reload.
        </p>
      </div>
    );
  }
}

export default App;

```