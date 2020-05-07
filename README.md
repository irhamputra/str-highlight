# str-highlight

the string for html, css and gql will be highlighted in JS

* npm
```bash 
npm i str-highlight
```
or

* yarn
```bash 
yarn add str-highlight
```



## Usage

#### HTML
```js
const htmlText = html`<p class="paragraph">Hello world<p>`
```

#### CSS
```js
const styles = css`
    items {
        color: red
    }
`
```

#### GraphQL
```js
const { gql } = require('str-highlight');

const query = gql`
    query {
        id
        name
    }
`

// pass your query to your GraphQL Client below
```

* with GraphQL Request
```js
// with GraphQL Request
const { request } = require('graphql-request')

request('https://api.graph.cool/simple/v1/movies', query).then(data =>
  console.log(data)
)
```
