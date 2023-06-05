### Questions

- [x] What are the key differences between functional components and class components in React?
- [x] Explain the concept of state in React. How is it different from props?
- [x] What is the purpose of the useEffect hook in React? Provide some examples of how you would use it.
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

- React Router is an external plugin that allow us to create navigation links and pages inside our web application. It works by adding an Provider that wraps all components with access to those specific routes.

- Virtual Dom is a copy or abstraction of the real DOM. React keeps track of every variable and state, manipulates the virtual DOM, then runs a diff against real DOM and batch only what it needs to be updated, instead of the whole HTML.

- I would deal with React form validation using controlled components with a local state. It allows us to implement real time validation and feedback and display usefull information to the user.

- React controlled components have their value storaged and updated on local state. So, React has knowledge and control every new data in the component, storing and updating it through setStates. Uncontrolled components are accessed directly in the real dom and update as well. Usually by using refs.

- Lifting state up in React is when you are changing a local state to its parent component, so other components have the same data, using this parent local state as a single source of true, passing data through props.

- Key prop identifies that single node from the entire virtual DOM and helps React to keep track of its content and information. It is very important for them to be unique as React will know exactly where it needs to update when batching after diff. If two elements have the same key, it will cause conflict of whom needs to be updated.

- The first one is updating components only when absolutely necessary. Avoiding prop drilling of nested components, as it will cause re-renders of every child component above, down the tree.Another option for optimization is to use contexts and provide a single source of true and allow access only for those who need it. Anoter alternative of optimization is to memoize components, keeping in the cache values that didn´t change.

- HOC is a technique to create a wrapper component that receives a target component as an argument, then execute some common logic and return the same component with extra data as props. One example of a HOC would be ....

- React hooks are functions that return data
