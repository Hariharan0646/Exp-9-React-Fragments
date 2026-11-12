# Exp 9 – React Lab Exercise: React Fragments

## NAME:  Hariharan S
## REG NO: 2305001009 

## Aim
To understand and implement React Fragments to group multiple JSX elements without creating unnecessary HTML elements in the DOM.

## Objectives
- Understand the concept of React Fragments.
- Use Fragment shorthand syntax.
- Use the explicit Fragment syntax.
- Group multiple JSX elements without an extra DOM node.
- Understand the difference between Fragments and div elements.

## Program

### Step 1: Create a React Project

```bash
npm create vite@latest react-fragments
cd react-fragments
npm install
npm run dev
```

Select React as the framework and JavaScript as the variant.

### Step 2: App.jsx – Using Fragment Shorthand

```jsx
function Student() {
  return (
    <>
      <h2>Student Details</h2>

      <h3>Name: Sukhmeet Kaur G</h3>

      <p>Register Number: 2305001032</p>

      <p>Department: Computer Science and Engineering</p>
    </>
  );
}

function App() {
  return (
    <>
      <h1>College Information System</h1>

      <Student />
    </>
  );
}

export default App;
```

### Step 3: Using Explicit Fragment Syntax

```jsx
import { Fragment } from "react";

function Student() {
  return (
    <Fragment>
      <h2>Student Details</h2>
      <p>Name: Sukhmeet Kaur G</p>
      <p>Department: CSE</p>
    </Fragment>
  );
}

function App() {
  return (
    <Fragment>
      <h1>College Information System</h1>
      <Student />
    </Fragment>
  );
}

export default App;
```

## Output

### Fragment Shorthand Syntax

<img width="1584" height="672" alt="Gemini_Generated_Image_dlr20pdlr20pdlr2" src="https://github.com/user-attachments/assets/3689fcc0-33ad-4120-b63f-668dbea1d1e5" />

### Explicit Fragment Syntax

<img width="1806" height="576" alt="Gemini_Generated_Image_yb91gqyb91gqyb91" src="https://github.com/user-attachments/assets/9be36570-9023-42b2-b386-412d3ab848ac" />


## Result

Thus, React Fragments were successfully implemented using shorthand and explicit syntax to group multiple JSX elements without creating unnecessary DOM elements.
