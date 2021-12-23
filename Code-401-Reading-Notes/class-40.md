# class_40
## Create a Next.js App
**build a complete web application with React from scratch**:
* Code has to be bundled using a bundler like webpack and transformed using a compiler like Babel.
* You need to do production optimizations such as code splitting.
* You might want to statically pre-render some pages for performance and SEO. You might also want to use server-side rendering or client-side rendering.
* You might have to write some server-side code to connect your React app to your data store.

### Next.js: The React Framework
Enter Next.js, the React Framework. Next.js provides a solution to all of the above problems.
<br>
Next.js aims to have best-in-class developer experience and many built-in features
* An intuitive page-based routing system
* Pre-rendering, both static generation (SSG) and server-side rendering (SSR) are supported on a per-page basis
* Automatic code splitting for faster page loads
* Client-side routing with optimized prefetching
* Built-in CSS and Sass support, and support for any CSS-in-JS library
* Development environment with Fast Refresh support
* API routes to build API endpoints with Serverless Functions
* Fully extendable

## React context
React context allows us to pass down and use (consume) data in whatever component we need in our React app without using props.

### When should you use React context?
These types of data include:

* Theme data (like dark or light mode)
* User data (the currently authenticated user)
* Location-specific data (like user language or locale)

### What problems does React context solve?
React context helps us avoid the problem of props drilling.
<br>
Props drilling is a term to describe when you pass props down multiple levels to a nested component, through components that don't need it.
