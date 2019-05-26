## Learned about Gatsby starters

Just like other frameworks such as rails we can generate a scaffold that provides us with the file structure and does alot behind the scenes.

`gatsby new hello-world https://github.com/gatsbyjs/gatsby-starter-hello-world`

`gatsby new [SITE_DIRECTORY_NAME] [URL_OF_STARTER_GITHUB_REPO]`

## Learned about JSX syntax

In react we can use HTML directly in our JavaScript components with the JSX syntax. It allows for creation of components that seem contained. I can see this having the benefit of a component being clear of what it contains.

## Learned about components

compoments are core to React. A component is a building block. Self contained chunks of code that are written in JSX.

## Learned about React “props” and reusing React components

```javascript
export default props => <h1>{props.headerText}</h1>
```

`header.js (this is a component we are building)`

```javascript
import React from "react"
import Header from "../components/header"

export default () => (
  <div style={{ color: `teal` }}>
    <Header headerText="About Gatsby" />
    <p>Such wow. Very React.</p>
  </div>
)
```

`about.js (this is the file we are importing the component into and then writing the content "headerText="about Gatsby")`

"Props" are properties that are passed into the React components. Props enable the components to be resuable.

## Links in Gatsby

```javascript
<Link to="/contact/">Contact</Link>
```

```javascript
import { Link } from "gatsby"
```

## CSS modules

A CSS Module is a CSS file in which all class names and animation names are scoped locally by default.

CSS Modules are very popular because they let you write CSS normally but with a lot more safety. The tool automatically generates unique class and animation names, so you don’t have to worry about selector name collisions.

Gatsby works out of the box with CSS Modules. This approach is highly recommended for those new to building with Gatsby (and React in general).
