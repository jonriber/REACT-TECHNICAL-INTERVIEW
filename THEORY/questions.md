### Questions

- What are the key differences between functional components and class components in React?
- Explain the concept of state in React. How is it different from props?
- What is the purpose of the useEffect hook in React? Provide some examples of how you would use it.
- How does React Router work? Explain its role in building single-page applications.
- What is the significance of the virtual DOM in React? How does it improve performance?
- How would you handle form input validation in a React component?
- What are controlled components in React? How do they differ from uncontrolled components?
- Explain the concept of lifting state up in React. When would you use this pattern?
- What is the purpose of the key prop in React? Why is it important when rendering lists of components?
- How can you optimize performance in a React application? Share some techniques or best practices.
- What is Redux, and why might you choose to use it in a React application? How does it work?
- Explain the concept of higher-order components (HOCs) in React. Provide an example of when you would use an HOC.
- What are React hooks? How do they differ from class-based lifecycle methods?
- How would you handle asynchronous operations, such as API calls, in a React component?
- Describe the process of deploying a React application to a production environment.

### Answers

- Class components are components built using class syntax. Further more, they all have built in methods called component lifecycle methods, which can modify data according to the current component lifecycle. Class components do have a render method, and uses this keyword to bind custom methods, handlers, local state and props. It´s necessary to call a class constructor to initialize local state and use props from parent components.<br/>
Functional components are components based in javascript function, which returns something, equivalent to the render method from class components. It doesn't require the use of this keyword anymore and you get a simple and shorter syntax to build components.

- State and props are a type of data. The biggest difference between both of them is that state is data managed locally (inside the component) and props is data received from a parent component, which means, data passed through.

- useEffect is a React hook that allow functional component lifecycle management. It is a conjunction of all other separeted class based components methods, into a single one, so, there you get to modify your components when it has mounted, updated or unmounted.<br/>
A common use case of this hook it to fetch external data (API) into your application, according to an array of dependencies.

