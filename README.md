# React Cheat Sheet

##### Wrapping App in Router
```
import React from 'react';
import ReactDOM from 'react-dom';
import { BrowserRouter as Router, Route} from "react-router-dom";
import './index.css';
import App from './App';
import registerServiceWorker from './registerServiceWorker';

const Routes  = () =>  (
    <Router>
        <Route path="/" component={App} />
    </Router>
);

ReactDOM.render(
    <Routes />, 
    document.getElementById('root'));
registerServiceWorker();
```

###### app.js layout
```
import React, { Component } from 'react';
import './App.css';
import Layout from './Layout/';

class App extends Component {
  render() {
    return (
      <div className="App">
       
        <Layout/>
        
      </div>
    );
  }
}

export default App;
```

###### Class Component
```
import React, { Component } from 'react'

export default class test extends Component {
  render() {
    return (
      <div>
        
      </div>
    )
  }
}

```
###### Functional Component
```
import React from 'react'

export default () => {
  return (
    <div>
      
    </div>
  )
}

```

###### Class Component with prop types
```import React, { Component } from 'react'
import PropTypes from 'prop-types'

export default class test extends Component {
  static propTypes = {
    prop: PropTypes
  }

  render() {
    return (
      <div>
        
      </div>
    )
  }
}
```

###### Class Component with lifecycle hooks
```
import React, { Component } from 'react'
import PropTypes from 'prop-types'

class componentName extends Component {
    constructor(props) {
        super(props)

    }

    componentWillMount() {

    }

    componentDidMount() {

    }

    componentWillReceiveProps(nextProps) {

    }

    shouldComponentUpdate(nextProps, nextState) {

    }

    componentWillUpdate(nextProps, nextState) {

    }

    componentDidUpdate(prevProps, prevState) {

    }

    componentWillUnmount() {

    }

    render() {
        return (
            <div>

            </div>
        )
    }
}

componentName.propTypes = {

}

export default componentName
```
