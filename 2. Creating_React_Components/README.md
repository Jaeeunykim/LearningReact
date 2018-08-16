## 2-1 리액트 컴포넌트를 만들기

### 1. Yarn start
### 리액트는 컴포넌트로 구성되어있다. 
### JSX란? 리액트 컴포넌트를 자바스크립트로 만든다

### App.js
```javascript
import React, { Component } from 'react';
import logo from './logo.svg';
import './App.css';

class App extends Component{
    reder(){
        return (
            <div className="App">
             <div className="App-hearder">
                  <img src={logo} className="App-logo" alt="logo" />
                  <h2> **원하는 문구를 작성해보세요** </h2>
                </div>
                <p className="App-intro">
                  To get stated, edit <code>src/App.js</code>and svae to reload.
                </p>
            </div>
        );
    }
}

export default App;

```