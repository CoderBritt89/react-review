### Remember

Answer these on your own, then compare answers as a group

1.  What is React?

  a javascript library for building user interfaces
  that prioritizes component based architecture and utilizes unidirectional data flow.


2.  What is create-react-app?

  c
  a package that creates a default boiler plate react application.

3.  What is Component Based Architecture?

    sections of code are broken into different components to keep code cleaner, reusable, and to easily identify when code is broken. 


4.  What is JSX?

    **HTML-like syntax for building components in React
    JSX looks like HTML but allows us to write HTML/Javascript right into the same file

5.  What is the virtual DOM?

  the virtual DOM is representational kept in sync with the real DOM where changes are sent before making it to live production.
  helps ensure code is working properly before sending to live production


  **light-weight copy of DOM stored in memory and synced with the "real" DOM through a process called reconciliation.

6.  What is unidirectional (one-way) data flow?

    Data flowing from Parent to child component only
    data has only one way of moving to other components
    waterfall

### Understand

Discuss these questions in pairs if you have a 4-person group

7.  Summarize what happens when you run `create-react-app my-app`

      initializes and creates the new react app and names it "my-app"

8.  Summarize the steps for forking and cloning a repo with an existing React app. How does this process differ from the process of creating a new React app on your laptop?

  fork and clone, cd into the repository where it is stored, npm install, npm start.

  when creating new you use npx instead of Npm


9.  Explain what this code does:

this is our child component that's receiving props
assigning the className based on what the prop is.

```jsx
import React from "react";

const Mentor = props => (
  <div className="mentor-container">
    <h1 className={props.title === "Lead Mentor" ? "lead" : ""}>Tim Biles</h1>
    <ul>
      <li>Fort Worth, TX</li>
      <li>My email address is timbilestimbiles@gmail.com</li>
    </ul>
  </div>
);

export default Mentor;
```

10.  Explain how data is passed from a parent component to a child component.

### Apply

Try these on your own, but work together if you start to get stuck.

11.  Use `create-react-app` to create a new React application called `student-directory`

12.  Use the code from `Mentor` above to create a new functional, stateless component called `User` with a list of friends. Hard code the list of friends, do not use state or props.

### Analyze, Evaluate, Create

Discuss these questions as a group

13. What are the benefits and drawbacks of using a tool like create-react-app?

14. Compare and contrast JSX with other templating options, such as those used in Angular or Vue

15. Compare and contrast one-way data flow with two-way data binding.
