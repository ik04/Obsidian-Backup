- Introduce yourself
## SSR in Next Js vs SSG in nextjs:
Server-Side Rendering (SSR) in Next.js involves rendering pages on each request, while Static Site Generation (SSG) generates HTML at build time. SSR is suitable for dynamic content, while SSG is great for static content or pages that don't change frequently.

##  What is Async await:
Async/Await is a syntactic feature in JavaScript that simplifies the handling of asynchronous code. It allows you to write asynchronous code in a more sequential and readable way. The `async` keyword is used to declare an asynchronous function, and the `await` keyword is used to pause the execution of the function until a promise is resolved. It's commonly used with Promises to handle asynchronous operations like fetching data, making the code more readable and easier to reason about.

case where await not needed:
**Parallel Execution Requirement:** If you have multiple independent asynchronous operations that can be executed in parallel and you don't need to wait for all of them to complete before proceeding, using `Promise.all` or other concurrency mechanisms might be more suitable.

## What is a Promise, and why did we need async await as a syntactic sugar ontop of a promise:

In JavaScript, a `Promise` is an object that represents the eventual completion or failure of an asynchronous operation and its resulting value. It is a way to handle asynchronous operations more easily and cleanly than using callbacks.

`async/await` is a syntactic sugar built on top of Promises to simplify the process of working with asynchronous code. It makes asynchronous code look and behave more like synchronous code, making it easier to read and write.

- Gimme example of a promise without an api call (optional)(scary topic)
- How do you abstract api keys in nextjs
- Explain your project 
- Get snippets ready for questions
- What is the Lamp stack
## what is Micro-service architecture, give me an example of a micro-service:

Microservices architecture is an approach to developing a software system as a collection of small, independent services, each running in its own process and communicating with lightweight mechanisms, often an HTTP or message-based protocol. Each service is designed to perform a specific business function and can be developed, deployed, and scaled independently. This architectural style contrasts with the traditional monolithic architecture where the entire application is developed and deployed as a single unit.
eg: stripe, captcha etc.

## What is the Hyper Text Transfer Protocol:
The HyperText Transfer Protocol (HTTP) is the foundation of data communication on the World Wide Web. It is an application layer protocol that enables the transfer of hypermedia documents, such as HTML. HTTP is the protocol used for communication between a client (such as a web browser) and a server (where the requested resources are hosted).


- What is the DOM
- What is the CssOM
- What is a Migration Script
## Name a Tool You would use if you didn't have Fetch Api or Axios to make the Api Call:
XHR


- Why Next tech lab
- what is your end goal with Web
- What is NextJs, how is it different from react
- Flexbox vs Grid when to use what


- Make An Api call in base js using a script tag and hydrate the output onto an h3 tag (optional)
https://jsonplaceholder.typicode.com/todos/1 (for api call)


- how would you render input from a form into a div using base js (if they can't answer the first)(file in prac)


- why use id sometimes, what can you do with it in certain cases. (random)
- what does the defer keyword do in the script tag

- why switch to react


- Explain to me how you would implement a Block Functionality in a FullStack website (Left join, in the most efficient way)

- What is Data Normalization, how does it improve scalability

- What is Database Indexing (optional)

- Give me an Application of ssr when making a site using nextjs

- What is useContext, how does it help with state transfer.

- show me an implementation of useContext in a react App or a Next app

- what is useEffect and what is the dependency array 



 Ask First if they've: used the tool
- What is useMemo, what are some drawback to using useMemo

- What is useCallBack

- useCallback vs useMemo

- how do you manage user sessions (context)

- token based authentication

- what is a middleware, how would you design a middleware to prevent unauthorized access

- what is cors

- how would you make a gallery application and how would you prevent a cors error from your server

- how would you ensure that all requests from your user session are authenticated (withCredentials true)

- how do you persist a user session in react or whatever they use







