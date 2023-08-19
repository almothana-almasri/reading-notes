[Back to Home](../README.md)

## Reading Class-39: React 3

**1. React Context:**
React Context is a feature for passing data through a React component tree without manual prop passing. It's useful for global state and data sharing.

**2. `useContext` Hook:**
`useContext` is a React Hook that lets functional components access data from a React Context. It avoids using `Context.Consumer`.

Example:

```jsx
import React, { useContext } from 'react';
import MyContext from './MyContext';

function MyComponent() {
  const contextValue = useContext(MyContext);
  return <p>Value: {contextValue}</p>;
}
```

**3. Next.js:**
Next.js is a React framework for server-rendered applications. It offers server-side rendering, routing, and performance optimization.

Example:
1. Create `pages/posts/[slug].js`.
2. Fetch post data based on slug.
3. Utilize `getStaticPaths` and `getStaticProps` for routing and data fetching.

```jsx
// pages/posts/[slug].js
function Post({ post }) {
  return (
    <div>
      <h1>{post.title}</h1>
      <p>{post.content}</p>
    </div>
  );
}

// getStaticPaths and getStaticProps functions here...

export default Post;
```

Next.js simplifies dynamic routing and server rendering for scalable web apps.




*- Author: Almothana Almasri*