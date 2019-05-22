# React

## build a react one page app

We will use the create-react-app package to create a react application.

```bash
create-react-app [name]-client-react
#to host the react project.
```

The package.json desribes the dependence relationship.  
Generally the react-app will be in localhost:3000.  
Everything under < /root> will be rendered dynamically injected __inmediatlly__.  
Everything will be finished in /src. index.js is the entry point from react point of view.  
Not all browers support ES6. like import. We will stick on the React.  
React.dom is speficing on the DOM.  Export the class the function and variables.  
React <-> React.DOM <-> Regular HTML.

React.DOM is only used in the index.js in the high level.

React use the jsx, the intermix of js and html.  

```js
export default App;
//in the in end of the react.js
//then others can take the function App to render.
```

### deploy the react app to heroku [TODO]

### Node.js

Node.js is a framework to run js on a server.  
npm: node package manager. Equivilent to maven.  
For the node world, download the packages from npm repository.

## React + BOOTSTRAP

```bash
npm install bootstrap
#if you want to update package.json

npm install bootstrap --save
```

Don't forget update the package.json.  Keep looking.  It's safer to copy than import directly.

Whiteboard.js

```js
import React from 'react'

export default class Whiteboard extends React.Component {
    render() {
        // can do any computation here and return in the return statement.
        return(
            // the top level should be always one element
            <div className = "container-fluid">
                <h1> WhiteBoard </h1>
            </div>
        )
    }
}
//the syntax of export is like the syntax of modifier like java.
```

## BOOTSTRAP CARDS & DECKS [More information on the github]

Create a card to provide small summaries.  
Style can take the json object as the css style. Even you can call a function in the style on the fly.

### parameterized Message component

constructor, super, props. pass the parameters to the compounent. 

### Creating a Stateless compounent

Pure function .
Only thing the function need to do is return.
No need constructor, no need render function.