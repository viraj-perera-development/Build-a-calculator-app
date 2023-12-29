"# Build-a-calculator-app" 

#TO RUN THIS APPLICATION:

paste "npm start" on your terminal

#TO EXERCISE:

-Steps1

Create an App.css file on your root folder and paste the following code:

* {
    font-family: sans-serif;
  }
  input,
  button {
    font-size: 20px;
    padding: 10px;
    border-radius: 5px;
  }
  input {
    display: block;
    margin-bottom: 20px;
  }
  button {
    border: 1px solid gray;
    background: whitesmoke;
    margin-right: 5px;
  }
  button:nth-last-child(2),
  button:nth-last-child(1) {
    background: tomato;
    color: white;
  }


-Steps2

Into your App.js file paste the following code:

import {
  useState,
  useRef
} from "react"; 
import "./App.css";

function App() { 
  const inputRef = useRef(null); 
  const resultRef = useRef(null); 
  const [result, setResult] = useState(0); 
 
  function plus(e) { 
    e.preventDefault(); 
    setResult((result) => result + Number(inputRef.current.value)); 
  }; 
 
  function minus(e) { 
  	// Add the code for the minus function 
  };
 
  function times(e) { 
    // Add the code for the plus function 
  }; 
 
  function divide(e) { 
    // Add the code for the divide function 
  };
 
  function resetInput(e) { 
    // Add the code for the resetInput function 
  }; 
 
  function resetResult(e) { 
  	// Add the code for the resetResult function 
  }; 
 
  return ( 
    <div className="App"> 
      <div> 
        <h1>Simplest Working Calculator</h1> 
      </div> 
      <form> 
        <p ref={resultRef}> 
          {/* add the value of the current total */} 
        </p> 
        <input
          pattern="[0-9]" 
          ref={inputRef} 
          type="number" 
          placeholder="Type a number" 
        /> 
        <button onClick={plus}>add</button> 
        {/* Add the subtract button */} 
        {/* Add the multiply button */} 
        {/* Add the divide button */} 
        {/* Add the resetInput button */} 
        {/* Add the resetResult button */} 
      </form> 
    </div> 
  ); 
} 
 
export default App; 

-Steps3

Complete the remaining functions and check it by running "npm start" on command line.
  