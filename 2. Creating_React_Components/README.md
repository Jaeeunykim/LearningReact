## 2-1 리액트 컴포넌트를 만들기

### 1. Yarn start
### 리액트는 컴포넌트로 구성되어있다. 
### JSX란? 리액트 컴포넌트를 자바스크립트로 만든다

```javascript
App.js

import React, { Component } from 'react';
import './App.css';
import Movie from './Movie';

class App extends Component{
  render(){
    return(
        <div className="App">
          <Movie />
          <Movie />
          <Movie />
          <Movie />
        </div>
    );
  }
}

export default App;

```

```javascript
Movie.js

import React, {Component} from 'react';
import './Movie.css';

class Movie extends Component{
    render(){
        return(
            <div>
                <MoviePoster />
                <h1>hello this is a movie</h1>
            </div>
        )
    }
}

class MoviePoster extends Component{
    render(){
        return(
            <img src = "https://steamcdn-a.akamaihd.net/steam/apps/416560/header.jpg?t=1504213621" />    
        )
    }
}

export default Movie


```

