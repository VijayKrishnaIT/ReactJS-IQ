# ReactJS-IQ

1. What is Component in React?
   Components are the building blocks of any React app. Components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.

2. What is DOM? What is Virtual DOM in react?
   DOM stands for Document Object Model.
   Virtual DOM is the virtual representation of the Real DOM.
   React uses virtual DOM to enhance its performance.
   A virtual DOM object has the same properties as a real DOM object, but it lacks the real thing's power to directly change what's on the screen.

3. Component Types?
   we have two types of Components.

   1. Stateless Components (Functional Components)
   2. Stateful Components (Class Level Components)

4. What are Functional Components?
   A functional component is just a plain JavaScript function which accepts props as an argument and returns a React element.

5. What is Class Level Components?
   A class component requires you to extend from React.Component and create a render function which returns a React element.

6. What is html?
   HTML is the standard markup language for Web pages.
   With HTML you can create your own Website.

7. What is CSS??
   CSS is a language that describes the style of an HTML document.
   CSS describes how HTML elements should be displayed.

8. In how many ways we can write CSS?
   There are three ways to apply CSS to HTML: Inline, internal, and external.
   Inline: <p style="color: red">text</p>
   Internal: Embedded, or internal, styles are used for the whole page. Inside the head element, the style tags surround all the styles for the page.
   External: External styles are used for the whole, multiple-page website. There is a separate CSS file.

9. Difference between Virtual DOM and DOM ?
   A virtual DOM object has the same properties as a real DOM object, but it lacks the real thing’s power to directly change what’s on the screen.
   Manipulating the DOM is slow. Manipulating the virtual DOM is much faster, because nothing gets drawn onscreen

10. Tell me different tags in HTML.

<!DOCTYPE>     Defines the document type
<html>    	   Defines an HTML document 
<head>    	   Contains metadata/information for the document 
<title>    	   Defines a title for the document 
<body>         Defines the document's body 
<h1> to <h6>   Defines HTML headings 
<p>    		   Defines a paragraph 
<br>    	   Inserts a single line break 
<hr>    	   Defines a thematic change in the content 
<! --    -->   Defines a comment 
  
11. How to create project in react.js? 
	npx create-react-app my-app 
	cd my-app 
	npm start 
  
12.	Difference between react js and react native. 
	react js --> React is a JavaScript library for building user interfaces. Used to develop web applications.

    react native --> React Native is a framework for building native applications using JavaScript. Used to develop Mobile apps.

    So, the syntax and workflow remain similar, but the components are different.

13. What is higher order component?
    connect is the predefined component.
    connect component technically called as HOC.
    HOC Stands for higher order component.
    connect component helps to dispatch and subscribe the reducer.

14. What is redux?  
    A Predictable State Container for JavaScript apps. It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test. On top of that, it provides a great developer experience, such as live code editing combined with a time traveling debugger.

15. What is box model in CSS?
    All HTML elements can be considered as boxes. In CSS, the term "box model" is used when talking about design and layout. The CSS box model is essentially a box that wraps around every HTML element. It consists of margins, borders, padding, and the actual content.

16. Different types of component in react js ?  
    Functional Components: Functional components are functions that takes in props and return JSX.
    Class Components: Class components use extends React.Component after declaring the class HelloWorld and requires a render() method to return JSX code
    Pure Components: Pure components are primarily used to provide optimizations. They are the simplest and fastest components we can write. They do not depend or modify the state of variables outside its scope. Hence, why pure components can replace simple functional components.
    Higher-Order Components: A higher-order component (HOC) is an advanced technique in React for reusing component logic.

17. Difference between class level component and functional component?
    The most obvious one difference is the syntax. A functional component is just a plain JavaScript function which accepts props as an argument and returns a React element.
    A class component requires you to extend from React.Component and create a render function which returns a React element.

18. How react work? What exactly is VIRTUAL DOM?
    ReactJS is View in MVC.
    Virtual DOM is a virtual representation of the real DOM.
    React uses virtual DOM to enhance its performance.

19. All the life cycle methods or hooks of REACT  
    Life cycle includes Mounting, Updating, and Unmounting.
    React class lifecycle methods, you can think of useEffect Hook as componentDidMount, componentDidUpdate, and componentWillUnmount combined.
    • componentWillMount is executed before rendering, on both the server and the client side.
    • componentDidMount is executed after the first render only on the client side. This is where AJAX requests and DOM or state updates should occur. This method is also used for integration with other JavaScript frameworks and any functions with delayed execution such as setTimeout or setInterval. We are using it to update the state so we can trigger the other lifecycle methods.
    • componentWillReceiveProps is invoked as soon as the props are updated before another render is called. We triggered it from setNewNumber when we updated the state.
    • shouldComponentUpdate should return true or false value. This will determine if the component will be updated or not. This is set to true by default. If you are sure that the component doesn't need to render after state or props are updated, you can return false value.
    • componentWillUpdate is called just before rendering.
    • componentDidUpdate is called just after rendering.
    • componentWillUnmount is called after the component is unmounted from the dom. We are unmounting our component in main.js.

20. What exactly shouldComponentUpdate return and how it works ?
    The shouldComponentUpdate() method checks the current props and state, compares it to the next props and state and then returns true if they are different, or false if they are the same.

21. What exactly when componentUnmount is Called?
    This method is called before the unmounting of the component takes place. Before the removal of the component from the DOM, ‘componentWillUnMount’ executes. This method denotes the end of the component’s lifecycle.

22. What is key? Did you see if we don’t use key what will happen?
    Keys help React identify which items have changed, are added, or are removed.  
    if we don’t use key --> React will default to using the index of an element as a key.

23. What this.state.bind(this) exactly do?
    bind() method creates a new function that, when called, has its this keyword set to the provided value, with a given sequence of arguments preceding any provided when the new function is called.

24. What will happen if we call setState inside render() ?
    Calling setState() here makes your component a contender for producing infinite loops. The render() function should be pure, meaning that it does not modify component state, it returns the same result each time it’s invoked, and it does not directly interact with the browser.

25. what ref is used for?
    Refs provide a way to access DOM nodes or React elements created in the render method.
    Managing focus, text selection, or media playback.
    Triggering imperative animations.
    Integrating with third-party DOM libraries.

26. difference of normal function and arrow function (this is from JavaScript)

        	normal function 						arrow function

    normal functions created using function declarations or expressions are constructible and callable.  
    Since regular functions are constructible, they can be called using the new keyword.
    arrow functions are only callable and not constructible, i.e arrow functions can never be used as constructor functions.

27. How we can add class in jquery?
    addClass() - Adds one or more classes to the selected elements.

28. What is call back function (JavaScript)
    Passing "one function" to "another function" as an argument called as "CallBack"

29. What is ajax and how it called (JavaScript)
    AJAX = Asynchronous JavaScript And XML.
    AJAX is not a programming language.
    AJAX just uses a combination of:
    A browser built-in XMLHttpRequest object (to request data from a web server)
    JavaScript and HTML DOM (to display or use the data)

30. What exactly promise return ?(JavaScript)
    Promises Establishes the communication between "producer" and "consumer". Promise return either Success or Failure.

31. if promise return failure then how you will catch the error?
    Using reject we will catch the error.

32. Difference between angular and react?  
     angular react

    1.  Angular is a complete framework.
    2.  Angular uses a two-directional data flow process where it updates the Real DOM directly 1. React is a JavaScript Library.  
         2. React updates only the Virtual DOM and is concerned with the one-directional data flow.

33. What is the need for redux?  
    Redux is used mostly for application state management. Redux maintains the state of an entire application in a single immutable state tree (object), which can’t be changed directly. When something changes, a new object is created (using actions and reducers).

34. How to manage state in redux?  
    By using Redux we’re solving this problem by introducing a central data store in our application. The store contains the state of the application and is the source of truth for components. By using the store concept, you do not need to synchronize state between components manually. Instead you can fully rely on the Redux store at any time.

35. Difference between state and props?
    In a React component, props are variables passed to it by its parent component.  
    State on the other hand is still variables, but directly initialized and managed by the component.

36. Why we use arrow functions?  
    Arrow functions acts like "callbacks" to receive the response from server.

37. Tell me about reduce() function?  
    reduce is a function that lets you reduce an array down to a single value. This value, which we’ll call the reduced value, can be any type you want such as a Map, Set, or any custom type defined by your project.

38. Difference between pure and impure components?
    In React, components are pure if their output is only determined by their inputs ( props ), and are impure if their output is determined by something other than the inputs, namely their state.

39. What is stateless component in react?  
    A stateless component is just a plain javascript function which takes props as an argument and returns a react element.

40. What is JSX in react?  
    JSX stands for JavaScript XML. JSX allows us to write HTML in React. JSX makes it easier to write and add HTML in React.

41. Explain the purpose of render() in React.  
    Render function in react.js is used to return the HTML you want to display in a component.
    Every Render function contains a return statement. This return statement can contain only one parent html tag.

42. Why we use routing?  
    React Router is a standard library for routing in React. It enables the navigation among views of various components in a React Application, allows changing the browser URL, and keeps the UI in sync with the URL.

43. How would you create Higher Order Components (HOCs) in React?  
    A higher-order component (HOC) is an advanced technique in React for reusing component logic.  
    a higher-order component is a function that takes a component and returns a new component.

44. What is the significance of keys in React?  
    Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity: const numbers = [1, 2, 3, 4, 5]; const listItems = numbers.

45. What is the significance of refs in React?  
    React Refs are a useful feature that act to reference a DOM element or a class component from within a parent component.

46. What are the differences between a class component and functional component?
    The most obvious one difference is the syntax. A functional component is just a plain JavaScript function which accepts props as an argument and returns a React element. A class component requires you to extend from React.Component and create a render function which returns a React element.

47. What is a higher order component?  
    HOC are a pattern that emerges from React’s compositional nature.
    Concretely, a higher-order component is a function that takes a component and returns a new component.

48. How Virtual-DOM is more efficient than Dirty checking?  
    The virtual DOM is used for efficient re-rendering of the DOM. This isn't really related to dirty checking your data.In fact, the diff algorithm is a dirty checker itself but it is used to see if the DOM is dirty instead.

49. What is render() in React? And explain its purpose?  
    Render function in react.js is used to return the HTML you want to display in a component.
    Every Render function contains a return statement. This return statement can contain only one parent html tag.

50. What are controlled and uncontrolled components in React?  
    In a controlled component, form data is handled by a React component. The alternative is uncontrolled components, where form data is handled by the DOM itself.

51. What are the life Cycle of ReactJS?

52. What are the Advantages of ReactJS?  
    ReactJS simplifies the overall process of scripting components.
    It facilitates advanced maintenance and boosts productivity.
    It guarantees quicker rendering

53. What do you know about synthetic events?

    SyntheticEvent, a cross-browser wrapper around the browser’s native event. It has the same interface as the browser’s native event, including stopPropagation() and preventDefault(), except the events work identically across all browsers.

54. What is difference between class and Functional Component?
    The most obvious one difference is the syntax.  
    A functional component is just a plain JavaScript function which accepts props as an argument and returns a React element.
    class component requires you to extend from React.Component and create a render function which returns a React element.

55. Explain Redux Flow?
    Redux allows you to manage the state of the application via a unidirectional flow where a child component can directly access the  
    state from the redux store instead of getting state changes from parent components.

56. Have you worked on React Hooks?
    They let you use state and other React features without writing a class.
    Hooks are backwards-compatible.
    Hooks are functions that let you “hook into” React state and lifecycle features from function components.  
    Hooks don’t work inside classes — they let you use React without classes.

57. Have you worked with Promise &Async, Await()?

    Promise can handle multiple asynchronous operations easily and provide better error handling than callbacks and events.
    Async and Await: Helps us to write the asynchronous code in a synchronous way. Async is infront of function.
    Await is inside a function marked as async.

    Promises Establishes the communication between "producer" and "consumer". Promise return either Success or Failure.  
    Using reject we will catch the error.  
    To consume the promise we call async and await instead of then(). Latest released in ES9.

58. How to perform async operations using redux?
    Async Operations. The Redux store supports strictly unidirectional and synchronous data flow. For asynchronous data flow, we need to apply some middleware to Redux.  
    This is done by enhancing createStore() with Redux's applyMiddleware() function, passing it the middleware to apply.

59. How did you test your application?
    There are a few ways to test React components. Broadly, they divide into two categories:
    Rendering component trees in a simplified test environment and asserting on their output.
    Running a complete app in a realistic browser environment (also known as “end-to-end” tests).

60. Which testing framework you have used and how code coverage % you were maintaining? JEST 100%
    Very fast performance. Compatible with React, VueJS, Angular and many projects.

61. What challenges you faced during development?
    Integration of WF, Proofing, building text editor using slate.js

62. Explain about your last project?
    CWB APP- Build a 1 stop shop for display content to capital ideas website.

63. What is debouncing?
    Forcefully stopping all the previous execution and considering latest request.
    Debouncing is not predefined. Ex: Bank ATM money withdraw and deposit.

64. Have you used redux-thunx?
    Redux Thunk(monitor actions) is a middleware that lets you call action creators that return a function instead of an action object.
    That function receives the store's dispatch method, which is then used to dispatch regular synchronous actions inside the body of the function once the asynchronous operations have completed.

65. Have you used redux-saga?
    Redux-saga(manipulating actions) is a redux middleware library, that is designed to make handling side effects in your redux app nice and simple. It achieves this by leveraging an ES6 feature called Generators, allowing us to write asynchronous code that looks synchronous, and is very easy to test.

66. Difference b/w Promise and Observable?

    Promise emits single value, Observable emits mutliple values extends RXJS.

67. Difference between angular and react
    Angular -->MVC React-->View in MVC , 10 times faster than angular because of virtual DOM.

68. ReactJS
    A JavaScript library for building user interfaces. React makes it painless to create interactive UIs.

69. Framework Vs Library
    Bootstrap and Angular are frameworks. If we Following certain Rules and Regulations is called the Framework.  
    JQuery, ReactJS are library. If we don't care about the rules and regulations then it is Library.

70. Event bubbling and Event Capturing?
    Event bubbling : The Events are propagating from down to top is called Event Bubbling.
    Event Capturing: Propagation of Events from top to bottom is called Event Capturing.

71. Stop propagation and Stop Immediate Propagation

    event.stopPropagation(); The event. stopPropagation() method stops the bubbling of an event to parent elements, preventing any parent event handlers from being executed.

    stopImmediatePropagation() method stops the rest of the event handlers from being executed. This method also stops the event from bubbling up the DOM tree.

72. Prevent Defaults
    The preventDefault() method cancels the event if it is cancelable, meaning that the default action that belongs to the event will not occur. For example, this can be useful when: Clicking on a "Submit" button, prevent it from submitting a form.  
    Clicking on a link, prevent the link from following the URL.

73. Type of null, object, array
    The typeof operator returns a string indicating the type of the unevaluated operand.
    typeof null; //object
    typeof {}; //object
    typeof []//object

74. How to check the API response is array or object?

    JSON objects and arrays are instances of JSONObject and JSONArray, respectively.  
    Add to that the fact that JSONObject has a get method that will return you an object you can check the type of yourself without worrying about ClassCastExceptions

75. Modules in react

    Creating a module means you will group a set of related components, methods and assets together, providing a public interface to be used by other modules.

76. Have you published any packages? No

77. let and const

    let : duplicate variables not allowed. let keyword is the block scoped member. Obeys scope rule.

    const: in const keyword "reinitialization" not possible. declare the variables. ES6

78. NPM packages
    A package is a file or directory that is described by a package.json file. A package must contain a package.json file in order to be published to the npm registry.  
    The react package contains only the functionality necessary to define React components. It is typically used together with a React renderer like react-dom for the web, or react-native for the native environments.

79. Unit Testing
    Unit Testing With Jest
    Jest is an open-source testing framework created by Facebook.  
    Jest offers the best integration with ReactJS including a command line tool for test execution.
    Jest also offers “snapshot testing” to verify the component rendering result.

80. What is debouncing? Forcefully stopping all the previous execution and considering latest request.
    Debouncing is not predefined. Ex: Bank ATM money withdraw and deposit.

81. What is HOC? Higher order Component
    connect is the predefined component.
    connect component technically called as HOC.
    HOC Stands for higher order component.
    connect component helps to dispatch and subscribe the reducer.

82. What is state management in react application? 3rd party module, with redux.

83. Redux? We have redux thux, redux saga.

84. What is redux thunx, redux saga? Inorder to monitor the store Actions(request, response) we go for thunk.

    Redux thunx is an outdated library. Saga is Advanced library for manipulating the actions.

85. Why Saga? In sagas debouncing is available by default.

86. What is store? Server is called as store. Store contains application with reducer.

87. What is reducer? Business logic

88. Request method is called Dispatch

89. Response method is called Subscribe.

90. Input parameters --> Actions.

91. What is addEventListerner --> Instead on onclick method we use.

92. HTML5 tags
<article>       Represents an independent piece of content of a document, such as a blog entry or newspaper article 
<aside >        Represents a piece of content that is only slightly related to the rest of the page. 
<audio>         Defines an audio file. 
<canvas>        This is used for rendering dynamic bitmap graphics on the fly, such as graphs or games. 
<command>       Represents a command the user can invoke. 
<datalist>      Together with the a new list attribute for input can be used to make comboboxes 
<details>       Represents additional information or controls which the user can obtain on demand 
<embed>         Defines external interactive content or plugin. 
<figure>        Represents a piece of self-contained flow content, typically referenced as a single unit from the main flow of the document. 
<footer>        Represents a footer for a section and can contain information about the author, copyright information, et cetera. 
<header>        Represents a group of introductory or navigational aids. 
<hgroup>        Represents the header of a section. 
<keygen>        Represents control for key pair generation. 
<mark>          Represents a run of text in one document marked or highlighted for reference purposes, due to its relevance in another context. 
<meter>        	Represents a measurement, such as disk usage. 
<nav>        	Represents a section of the document intended for navigation. 
<output>        Represents some type of output, such as from a calculation done through scripting. 
<progress>      Represents a completion of a task, such as downloading or when performing a series of expensive operations. 
<ruby>        	Together with <rt> and <rp> allow for marking up ruby annotations. 
<section>       Represents a generic document or application section 
<time>        	Represents a date and/or time. 
<video>        	Defines a video file. 
<wbr>        	Represents a line break opportunity.

93. What is document.write()? To write something on the webpage like tables

94. How to convert Object to string? JSON.Stringfy()

95. What is mandatory lifecycle in React? render ()

96. How to take state in react? With help of Constructor (){}

97. How to solve error? With help of break points F8. (reverse engineering), F10 line by line execution.

98. What is axios module? We can make network call with axios.
    "axios" is the 3rd module, used to make the Asynchronous calls in react applications.
    we will download axios module by using "yarn" tool.

    > cd axios-ex
    > yarn add axios --save

99. How to create REST API? Using Express.

100.  Why Callbacks? Through callbacks we can share data from child component to parent component.

101.  transition : all 1s

transform: translateX(50px); (moving to right side)

transform: translateX(-50px); (moving to left side)

transform: translateY(50px); (moving down)

transform: translateY(-50px); (moving up)

transfrom: skewX(45deg);

transform: skewX(-45deg);

transform: skewY(45deg);

transform: skewY(-45deg);

transform: scale(1.2,1.2); (for zooming)

transform: scale(1.2,1.2) rotate(20deg); (for zooming and rotating)

transform: perspective(100px) rotateY(10deg);

animation : xyz 1s infinite alternate;

@keyframe xyz{ }

{transform : translateY(-50px) transform:translateY(50px)}

Making the all spans under one group --> display : inline-block

99. 2-way Data binding: Delete in database and front end at a time.

100. What is element position Static, relative, fixed, absolute?


    The position property specifies the type of positioning method used for an element
    (static, relative, fixed, absolute or sticky).

    position: static; HTML elements are positioned static by default. Static positioned elements are not affected by the top, bottom, left, and right properties.

    position: relative; An element with position: relative; is positioned relative to its normal position.

    position: fixed; An element with position: fixed; is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled.

    position: absolute;An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).

102. What is border and margin?


    Margin: Clears an area outside the border. The margin is transparent.

    Border: A border that goes around the padding and content

    Content - The content of the box, where text and images appear

    Padding - Clears an area around the content. The padding is transparent

103. HTML5 API
     The HTML Geolocation API is used to locate a user's position.

104. Latest tags in HTML5

<article>       Represents an independent piece of content of a document, such as a blog entry or newspaper article 
<aside >        Represents a piece of content that is only slightly related to the rest of the page. 
<audio>         Defines an audio file. 
<canvas>        This is used for rendering dynamic bitmap graphics on the fly, such as graphs or games. 
<command>       Represents a command the user can invoke. 
<datalist>      Together with the a new list attribute for input can be used to make comboboxes 
<details>       Represents additional information or controls which the user can obtain on demand 
<embed>         Defines external interactive content or plugin. 
<figure>        Represents a piece of self-contained flow content, typically referenced as a single unit from the main flow of the document. 
<footer>        Represents a footer for a section and can contain information about the author, copyright information, et cetera. 
<header>        Represents a group of introductory or navigational aids. 
<hgroup>        Represents the header of a section. 
<keygen>        Represents control for key pair generation. 
<mark>          Represents a run of text in one document marked or highlighted for reference purposes, due to its relevance in another context. 
<meter>        	Represents a measurement, such as disk usage. 
<nav>         	Represents a section of the document intended for navigation. 
<output>        Represents some type of output, such as from a calculation done through scripting. 
<progress>      Represents a completion of a task, such as downloading or when performing a series of expensive operations. 
<ruby>        	Together with <rt> and <rp> allow for marking up ruby annotations. 
<section>       Represents a generic document or application section 
<time>        	Represents a date and/or time. 
<video>        	Defines a video file. 
<wbr>        	Represents a line break opportunity. 
  
105. Application cache? 
	An application cache provides the following benefits: Offline browsing: users can navigate a site or 
	use a web application although they are offline. Speed: cached resources are local, and therefore load faster.  
	Reduced server load: the browser only downloads resources that have changed from the server. 
  
106. Local Storage and Session Storage? Why? 
	Both localStorage and sessionStorage offer advantages compared to using cookies:  
	The data is saved locally only and can't be read by the server, which eliminates the security issue that cookies present.  
	It allows for much more data to be saved (10Mb for most browsers). 
  
	localStorage and sessionStorage allow to save key/value pairs in the browser. ...  
	Unlike cookies, web storage objects are not sent to server with each request.  
	Because of that, we can store much more. Most browsers allow at least 2 megabytes of data (or more)  
	and have settings to configure that. 
 
107. Why react famous ?? 
	ReactJS has become highly popular because of its extra simplicity and flexibility.

108. Why react-redux? used to integrate redux to react application

109. how to separate the actions? redux-thunx
110. Why redux-thunx? used to separate and manage the actions.

111. How to connect to server? axios.
112. Why axios? axios module used to make the rest api calls.

113. Virtual DOM
     Virtual DOM is a virtual representation of the real DOM.
     React uses virtual DOM to enhance its performance.
     A virtual DOM object has the same properties as a real DOM object, but it lacks the real thing's power to directly change what's on the screen.

114. How does Redux works


    The way Redux works is simple. There is a central store that holds the entire state of the application. Each component can access the stored state without having to send down props from one component to another. There are three building parts: actions, store, and reducers.

    Reducer --> Business Logic
    Payload--> Action
    Store --> Main Server
    Dispatch --> Request
    Response --> Subscribe
    State--> Store Component Data.

115. Lifecycle of React
     a. componentWillMount is executed before rendering, on both the server and the client side.


    b. componentDidMount is executed after the first render only on the client side. This is where AJAX requests and DOM or state updates should occur. This method is also used for integration with other JavaScript frameworks and any functions with delayed execution such as setTimeout or setInterval. We are using it to update the state so we can trigger the other lifecycle methods.

    c. componentWillReceiveProps is invoked as soon as the props are updated before another render is called. We triggered it from setNewNumber when we updated the state.

    d.	shouldComponentUpdate should return true or false value. This will determine if the component will be updated or not. This is set to true by default. If you are sure that the component doesn't need to render after state or props are updated, you can return false value.

    e.	componentWillUpdate is called just before rendering.

    f.	componentDidUpdate is called just after rendering.

    1.	componentWillUnmount is called after the component is unmounted from the dom. We are unmounting our component in main.js.

116. What is connect HOC?
     A higher-order component (HOC) is an advanced technique in React for reusing component logic. HOCs are not part of the React API. They are a pattern that emerges from React’s compositional nature.
     Concretely, a higher-order component is a function that takes a component and returns a new component.

117. What is Component?  
     Reusable portion of Complex UI Called as Component.
     As a React Developer, we can reuse Components.
     we can call React Applications are Component Based Applications.
     we have two types of Components.


    1) Stateless Components (Functional Components)

    2) Stateful Components (Class Level Components)

    The most obvious one difference is the syntax.
    A functional component is just a plain JavaScript function which accepts props as an argument and returns a React element.
    A class component requires you to extend from React.Component and create a render function which returns a React element.

118. Pure components
     Pure components are primarily used to provide optimizations. They are the simplest and fastest components we can write. They do not depend or modify the state of variables outside its scope. Hence, why pure components can replace simple functional components.

119. What is Saga, Thunk middleware
     we can implement session management (services implementation) by using "saga" , "thunk" and "redux".
     "saga" , "thunk" and "redux" are the 3rd party libraries.


    Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store's dispatch method, which is then used to dispatch regular synchronous actions inside the body of the function once the asynchronous operations have completed.

    Redux-saga is a redux middleware library, that is designed to make handling side effects in your redux app nice and simple. It achieves this by leveraging an ES6 feature called Generators, allowing us to write asynchronous code that looks synchronous, and is very easy to test.

120. How do you dispatch actions?
     dispatch an action from component, first connect it with the store and use the connect method of react-redux.
     Then, when you start to have logic in your mapDispatchToProps function, it's time to dispatch action in your saga.

121. What is react hooks ?
     Hooks are functions that let you “hook into” React state and lifecycle features from function components. Hooks don't work inside classes — they let you use React without classes. ... You can also create your own Hooks to reuse stateful behavior between different components.

122. Context Api
     React Context API is a way to essentially create global variables that can be passed around in a React app. This is the alternative to "prop drilling", or passing props from grandparent to parent to child, and so on. Context is often touted as a simpler, lighter solution to using Redux for state management.
     Context provides a way to pass data through the component tree without having to pass props down manually at every level.

123. tell me about current project?

124. Difference b/w angular vs react
     React
125. A JavaScript library for building user interfaces.

     - React is the UI Library.
     - React given by facebook.
     - React categorized into two subjects.
       1. ReactJS
       2. React Native
     - ReactJS, used to create the web applications.
     - React Native used to develop the mobile applications.
     - we will develop ReactJS Applications by using JSX.

     - JSX stands for JavaScript and XML.
     - Babel is the tool, used convert the XML to JavaScript.
     - Babel tool is the inbuilt tool of react library.
     - React follows the following principles.
       1. Simplifies the Complex UI
       2. Virtual DOM
     - because above principles react applications are faster applications.
     - React applications are Component Based Applications.
     - These Components are Reusable.
     - "Material-UI" is the library released by Facebook, used to increase the look and feel of react applications.
     - we can implement session management (services implementation) by using "saga" , "thunk" and "redux".
     - "saga" , "thunk" and "redux" are the 3rd party libraries.

     Angular

     1. Angular is the framework.
     2. Angular used to develop the web applications and mobile applications.
     3. we will develop angular applications by using TypeScript.
     4. TypeScript is the superset of JavaScript(TS is advanced JavaScript).
     5. we will install TypeScript by using following command.
        > npm install -g typescript@latest ( typescript@3.9.5 )

     - we will save TypeScript files by using ".ts" extension.

126. what is 2-way binding in angular or react?
     The two-way data binding technique allows the changes in View to update in the Model.


    - It uses a combination of property "[]" and event "()" binding.
    - The directive "ngModel" is responsible for handling the property and event binding for any specific element.
    - ngModel is defined in "formsModule" of "angular/forms" library.
    syntax:
    =======
    [(ngModel)] = "property"
    - property is a reference where data is updated.


    In one-way Binding the model data is updated to the view but any change in the View will not update the Model.
    - It is a read only technique often called as "interpolation".
    - The model data is Binded to view by using databinding "{{}}" expression.
    Note:
    =====
    Interpolation will not use any property Binding. It Binds value to any attribute directly by using "{{}}" databinding expression.

126. what is JSX & how browser read JSX??
     JSX stands for JavaScript and XML.


    - Babel is the tool, used convert the XML to JavaScript.
    - Babel tool is the inbuilt tool of react library.

127. What is purpose of render()?
     Render function in react.js is used to return the HTML you want to display in a component. Every Render function contains a return statement. This return statement can contain only one parent html tag.

128. Component? How to ambend(mix) 2 or more components? How? Yes create 2 components and merge using another component.


    Reusable portion of Complex UI Called as Component. As a React Developer, we can reuse Components.
    we can call React Applications are Component Based Applications.
    we have two types of Components.

    1) Stateless Components (Functional Components)

    2) Stateful Components (Class Level Components)

129. difference b/w state and props?  
     State
1. state is the predefined object in react library
1. state used to store the component data.
1. we will define state by using "state" keyword
1. "state" keyword is the predefined keyword.
1. constructor is the best place to define the state


    Props
    1.	"props" is the predefined property in react library.
    2.	 "props" used to receive the data from 3rd party resources
    (Components, Redux, Saga, Thunk,.....
    3.	“Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another.
    4.	“props” are basically kind of global variable or object.
    5.	The data in states and props are used to render the Component with dynamic data.
    6.	Props are passed to components via HTML attributes.
    7.	We can say, props are immutable (unable to be changed).

130. What is arrow function in react?
     Anonymous Functions / Arrow Functions / Fat Arrow Functions / CallBack Functions
     Arrow functions acts like "callbacks" to receive the response from server.
     The function without name called as "Anonymous Functions".
     from ES6 onwards, we can call "Arrow Functions".
     we will represent Arrow Functions by using "()=>{}"
     Arrow functions are "secured" compared to named functions.

131. In component stateful Vs stateless component(easy to test, what comes in)?
     we have two types of Components.


    1) Stateless Components (Functional Components)
    2) Stateful Components (Class Level Components)

    The most obvious one difference is the syntax.
    A functional component is just a plain JavaScript function which accepts props as an argument and returns a React element.
    A class component requires you to extend from React.Component and create a render function which returns a React element.

132. What is Refs in react?


    "ref" is the attribute used to assign logical name to DOM Elements.

    1. The "ref" is used to return a reference to the element.

    2. "ref" is used when we want to add methods to the components.

    3. "ref" act as an id.

    4. Example:
    	<input value = {this.state.data}

    	onChange = {this.updateState}

    	ref = "myInput">

    	</input>

    5. If "ref" points to a "standard component" (DOM node, such as input, select, div etc) then to retrieve the element; we just need to call "this.refs.ref".

    6. If "ref" points to a "composite component". we need to use the new ReactDOM module like "ReactDOM.findDOMNode(this.refs.ref)".

133.  What is Synthetic event?
1.  "Synthetic Events" is a cross-browser wrapper around the browser's native event.
1.  React implements a "synthetic event" system that brings consistency and high performance to react applications and interfaces.

1.  difference between flux and redux?

                                   Flux

1.  Flux is a JavaScript architecture or pattern for UI which runs on a unidirectional data flow and has a centralized dispatcher.
1.  It was created by Facebook, and complements React as view. Flux is a pattern
1.  In Flux, an action is a simple JavaScript object, and that's the default case in Redux too, but when using Redux middleware, actions can also be functions and promises.
1.  Flux is a pattern for managing how data flows through a React application.
1.  It is a method of working with React components is through passing data from one parent component to it's children components.

        						Redux

1.  Redux is a library.
1.  Redux is an open-source JavaScript library for managing application state.
1.  It is most commonly used with libraries such as React or Angular for building user interfaces.
1.  Redux is a predictable state container for JavaScript applications. It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test.
1.  it helps you manage the data you display and how you respond to user actions.

1.  Components of redux? action, reducer, container, component


    Components in redux
    				Actions
    				Store
    				Reducers
    				Dispatch
    				Subscribe
    				State
    				getstate()

    	Actions :
    Simply we call that actions are events.
    They are the only way we can send data from application to Redux store. The data can be from user interactions, API calls, or even form submissions.
    ➢ Actions are sent using the store.dispatch() method.
    ➢ Actions are plain JavaScript objects, and they must have a type property to indicate the type of action to be carried out.
    ➢ They must also have a payload that contains the information that should be worked on the action.

    Store:
    The store holds the application state.
    There is only one store in any Redux application.
    redux has one global store

    Reducers:
    ➢ Reducers are a pure function in Redux, these Pure functions are predictable.
    ➢ Reducers are the only way to change states in Redux.
    ➢ It is the only place where you can write logic and calculations.
    ➢ reducers main job is to take “current state” and an” action “ and return the ”new state”

    Dispatch:
    •	It allows to dispatch an action to change a state in your application.
    •	Dispatch() is the only way to trigger a state change.
    •	The store's reducing function will be called with the current getstate() result and the given action synchronously.
    •	It return value will be considered the next state.

    Subscribe:
    It helps to register a callback that Redux store will call when an action has been dispatched.
    As soon as the Redux state has been updated, the view will re-render automatically.

    State:
    state used to store the component data.

    getstate()
    Returns the current state tree of your application. It is equal to the last value returned by the store's reducer.
    and getstate() returns current state tree of your application.



136. how you are calling the backend? Async await and fetch
     To consume the promise we call async and await instead of then(). Latest released in ES9.
     because of callbacks code readability decreased, so in ES9 they introduced "async & await" keywords

137. did you build application from scratch? Yes cwb, discover etc.

138. how you are writing the test cases in react? JEST
     • Jest is the tool, used to write the unit test cases to "react" and "vue" applications.
     • we will install jest tool by using following command.
     • yarn add react-test-renderer --save
     • all the testing files have the ".test.js" extension.
     • we will test unit test cases by using "yarn test" or "jest"

139. how do you deploy the applications in QA? Backend team does the deployment.

140. Where do you apply deployment. On the Release branch we deploy the application.

141. do u use node.js? no

142. What is React-redux?


    react-redux module used to integrate the redux architecture to react application.

143. Explain redux react ?
     Redux is a predictable state container for JavaScript apps.
     It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test. ... You can use Redux together with React, or with any other view library.

144. restful explain?
     REST or RESTful API design (Representational State Transfer) is designed to take advantage of existing protocols. While REST can be used over nearly any protocol, it usually takes advantage of HTTP when used for Web APIs. …

145. promises?


    - Promises Establishes the communication between "producer" and "consumer".
        - Promises also called as "special javascript objects".
        - we will create Promises by using "Promise" class constructor.
        - Promises have 3 states
            1) success  (resolve)
            2) error    (reject)
            3) pending
        - we will consume promises by using "then()"

146. dependency injection?
     Communication between the component and Services is called DI.
     Services
1. Predefined Services – service given by Angular Framework.
1. Custom Services – Services given by user.

1. How do you pass from Child to Parent? Parent to Child ?


    Parent to Child 	pass from Child to Parent
    Props are passed from parent component to child components.

    Props is also a plain JavaScript object. Props is immutable, which means its values can NOT be changed. Passing data from the child components to the parent components is more complicated, but also requires props. Props can only pass data from parent to child. This time, instead of passing a variable, we will be passing a function or callback to the child components.
    Props are passed from parent component to child components.

    Passing data from the child components to the parent components is more complicated, but also requires props. Props can only pass data from parent to child. This time, instead of passing a variable, we will be passing a function or callback to the child components.


148. Why is super keyword used?
     "super" keyword is used as a “function” which calls the parent class. The super() in JavaScript is used to call the methods of the parent class. It is used within a constructor function to call the parent constructor function.

149. Why can't we use setstate directly?


    state is mutable(can change).The value of state properties can be change by using setState.

150. What is use of provider?

     By using provider in index.js we can make store available globally.
     The <Provider/> makes the redux store globally
     ReactDOM.render(<Provider store = {store}><App/></Provider>,document.getElementById(‘root’));

151. can we have more than 1 store?
     multiple stores are unnecessary in Redux (except for performance edge cases which you are supposed to profile first anyway).
     Flux background will assume multiple stores is the solution to making update code modular.

152. What are generator functions? why? What is yield?
     Generators are used to control the flow of application inside the function call.
     Generators are also introduced in ES6.
     Generators functions should have the "\*"
     to control the application flow we will take "yield" keyword.

153. What is rest operator and spread operator?
     The spread operator allows us to spread the value of an array (or any iterable) across zero or more arguments in a function or elements in an array (or any iterable). The rest parameter allows us to pass an indefinite number of parameters to a function and access them in an array.

154. how can you make the copy for the object?
     To copy an object in JavaScript, you have three options:
     Use the spread (...) syntax
     Use the Object.assign() method
     Use the JSON.stringify() and JSON.parse() methods

155. difference let and var?
     Var- variables. Duplicate values allowed, global scope member
     Let - Es6 Duplicate variables not allowed, block scope member
     Const - Es6, reinitialization not possible, declare variables

156. what is function prototyping?
     function prototype specifies the input/output interlace to the function i.e. what to give to the function and what to expect from the function.

157. what is closure? Example?


    - if any inner function holding the outer function data, then such scenario called as closure.
    <script>
    function fun_one(){
        var x = 10;
        var y = 20;
        return ()=>{
            console.log(x);
            console.log(y);
        }
    };
    console.dir( fun_one() );  //0: Closure (fun_one) {x: 10, y: 20}
    </script>

158. how can you remove the duplicate elements from array?
     Remove duplicates from an array using a Set
     Remove duplicates from an array using indexOf() and filter() methods
     Remove duplicates from an array using forEach() and include()

159. what are the side effects of saga middleware?
     redux-saga is a middleware library for Redux that handles asynchronous actions triggered in your application. Often referred to as 'side effects', these events are outside of the main flow of your application's functionality, and in turn outside of your control.

160. what are higher order components?
     A higher-order component (HOC) is an advanced technique in React for reusing component logic.
     They are a pattern that emerges from React's compositional nature.  
     Concretely, a higher-order component is a function that takes a component and returns a new component.

161. git merge and rebase?
     rebase a feature branch onto master, you move the base of the feature branch to master branch's ending point.
     Merging takes the contents of the feature branch and integrates it with the master branch. As a result, only the master branch is changed. Merging adds a new commit to your history.

162. Why Saga?


    - Sagas created by using “generator” functions.
    - Sagas takes advantage of the “yield” keyword to halt execution within a function.
    - Easy to test
    - It is useful to express complex application logic.


163.What is class level component and functional level component? differences?
The most obvious one difference is the syntax. A functional component is just a plain JavaScript function which accepts props as an argument and returns a React element.  
 A class component requires you to extend from React.Component and create a render function which returns a React element.

164. What are lifecycle methods in react?


    life cycle include Mounting, Updating, and Unmounting.
    React class lifecycle methods, you can think of useEffect Hook as componentDidMount, componentDidUpdate, and
    componentWillUnmount combined.
    •	componentWillMount is executed before rendering, on both the server and the client side.
    •	componentDidMount is executed after the first render only on the client side. This is where AJAX requests and DOM or state updates should occur. This method is also used for integration with other JavaScript frameworks and any functions with delayed execution such as setTimeout or setInterval. We are using it to update the state so we can trigger the other lifecycle methods.
    •	componentWillReceiveProps is invoked as soon as the props are updated before another render is called. We triggered it from setNewNumber when we updated the state.
    •	shouldComponentUpdate should return true or false value. This will determine if the component will be updated or not. This is set to true by default. If you are sure that the component doesn't need to render after state or props are updated, you can return false value.
    •	componentWillUpdate is called just before rendering.
    •	componentDidUpdate is called just after rendering.
    •	componentWillUnmount is called after the component is unmounted from the dom. We are unmounting our component in main.js.


165. What is React-redux? Why?
     used to integrate redux architecture to react application

166. What is Hoisting in JS?
     Hoisting is the JavaScript interpreter's action of moving all variable and function declarations to the top of the current scope. However, only the actual declarations are hoisted

167. What is event bubbling and event capturing?
     The Events are propagating from down to top is called Event Bubbling.
     Propagation of Events from top to bottom is called Event Capturing.
     Id is logical name, id help in implementing the event bubbling or event capturing.

168. event delegation
     JavaScript event delegation is a simple technique by which you can add a single event handler to the parent instead of adding same event handler to his multiple child elements.

169. Where code hosted? Bitbucket


    React Latest Hooks

        useState

        UseEffect

    useMemo

    What is a Hook? A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.

    What does calling useState do? It declares a “state variable”. This is a way to “preserve” some values between the function calls — useState is a new way to use the exact same capabilities that this.state provides in a class. Normally, variables “disappear” when the function exits but state variables are preserved by React.

    What does useEffect do? By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates. In this effect, we set the document title, but we could also perform data fetching or call some other imperative API.

    What is useMemo do?
    Returns a memoized value.
    Pass a “create” function and an array of dependencies. useMemo will only recompute the memoized value when one of the dependencies has changed. This optimization helps to avoid expensive calculations on every render.
