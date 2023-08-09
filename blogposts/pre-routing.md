---
title: 'Routing'
date: '2023-03-14'
---


<!-- [Local Image](/public/images/next-vs-reactjs3.jpeg) -->

**ReactJS**: 
- ReactJS is a JavaScript library for building user interfaces. It focuses primarily on the "view" layer of an    application and doesn't provide built-in solutions for handling routing.
- If you want to implement routing in a React application, you typically need to use additional libraries, with React Router being one of the most commonly used choices. 
- React Router provides a declarative way to define the routes of your application and render different components based on the current route.

**Example:**
```
import React from 'react';
import { BrowserRouter as Router, Route, Switch } from 'react-router-dom';
import Home from './components/Home';
import About from './components/About';
function App() {
  return (
    <Router>
      <Switch>
        <Route exact path="/" component={Home} />
        <Route path="/about" component={About} />
      </Switch>
    </Router>
  );
}
export default App;
```

**Next.js:**
- Next.js is a framework built on top of React that adds a layer of features for server-rendered applications, static site generation, and routing. 
- One of the notable features of Next.js is its built-in routing system. With Next.js, you don't need an external library like React Router to handle routing. 
- Next.js provides a file-based routing system, where you can create files in a specific directory to define your routes. The files are automatically mapped to corresponding routes.

**Example:**
```
/pages
  /index.js (maps to '/')
  /about.js (maps to '/about')
```
Next.js's file-based routing simplifies the process of setting up routes, and it's tightly integrated with the other features that Next.js offers, like server-side rendering and static site generation.


