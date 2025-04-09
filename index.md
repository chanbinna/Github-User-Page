# Chanbin's User Page

**Software Engineer | Full Stack Developer | AI Enthusiast**
📧 [chna@ucsd.edu](mailto:chna@ucsd.edu) | 🌐 [devchanbin.vercel.app](https://devchanbin.vercel.app)  | 🔗 [LinkedIn](https://linkedin.com/in/chanbin-na/) | 💾 [GitHub](https://github.com/chanbinna)

![Profile](/image/profile.jpeg)

## Introduction
Hi! I'm **Chanbin Na**, a Mathematics–Computer Science student at UC San Diego with a strong interest in full-stack web development. I enjoy turning ideas into real applications—whether it's building responsive frontends, secure backends, or working on team projects. I'm always learning and excited to grow as a developer through hands-on experience and collaboration.

---

## Table of Contents

1. [Education](#education)
2. [Technical Skills](#technical-skills)
3. [Experience](#experience)
4. [Projects](#projects)
5. [Leadership](#leadership)
6. [To-Do List](#to-do-list)

---
## Technical Skills
- **Languages**: Java, Python, JavaScript, C/C++, C#, HTML/CSS, Bash, GraphQL
- **Frameworks**: React, Next.js, Node.js, Express, Flask, .NET Core, Reflex
- **Tools**: Git, Docker, Vercel, IntelliJ, VS Code, Figma, Google Gemini API
- **Databases**: MongoDB, MySQL
- **Libraries**: pandas, NumPy, OpenCV, scikit-learn, Socket.IO

---

## Education

> **University of California, San Diego**  
> *B.S. Mathematics–Computer Science, Minor in Data Science (Jun. 2025)*  
> Relevant Courses:  
> - Data Structures  
> - Algorithms  
> - Software Engineering  
> - ML Foundations  
> - Theory of Computation  
> - Optimization  

---

## Experience

### Darc Korea Association
**Full Stack Engineer** — Seoul, South Korea *(Jun 2024 – Sep 2024)*  
- Developed a 26-page full-stack application for a nonprofit  
- Built a secure admin panel (bcrypt login) and dynamic form handling  
- Deployed on Vercel, optimized for SEO  
- 🔗 [darc-incheon.com](https://www.darc-incheon.com)

### Y STEM and Chess Inc.  
**Software Engineer Intern** — Remote *(Mar 2024 – Jul 2024)*  
- Developed a new website using React and Node.js  
- Maintained and extended features in a legacy Angular/Docker system  

### Republic of Korean Army  
**Squad Leader, Signaller** — Seoul, South Korea *(Dec 2020 – Jun 2022)*  
- Led a 10-member networking unit  
- Deployed and maintained LAN, Ethernet, and cellular network systems 

---

## Projects

### StitchWitch: Generative AI Surgery Assistant (2024)

**Tech Stack**: Google Gemini Pro, Reflex, OpenCV
- Developed an AI-powered application for real-time surgical error detection
- Integrated prompt-engineered Gemini agents with medical protocols using the Reflex framework
- Pitched the project at LA Hacks to companies including Google, Intel, and Fetch AI
  
### STUDYSPHERE (2024)
**Tech Stack**: React, Node.js, Express.js, MySQL, Socket.IO
- Built a study group matching platform ranked in the top 10 at the 2024 LIKELION US Hackathon
- Developed real-time group chat, video call, and matching functionality
- Led a team of five developers and managed GitHub issues, pull requests, and deployments

### Roommate Matcher – ACM (2023)
**Tech Stack**: TypeScript, React, Express.js, MongoDB
- Led frontend development using React and managed state-driven components
- Built the backend using Express.js with MongoDB for storing user profiles and matching preferences

---
## Leadership

### Vice President — LIKELION @ UCSD (Feb 2024 – Present)
- Coordinated student project teams and managed project timelines and recruitment
- Delivered weekly technical workshops on the following topics:
  - HTML, CSS, JavaScript
  - React, Next.js, GraphQL
  - MongoDB
- Supported beginners in completing web projects through mentorship and code reviews
- Project site: [LIKELION Beginner Series](https://likelion-ucsd-beginner-project.vercel.app/en)

#### Basic React Example from workshops
```jsx
import React, { useState } from "react";

function App() {
  // State to store the list of tasks
  const [tasks, setTasks] = useState([]);
  const [task, setTask] = useState("");

  // Function to add a task to the list
  const addTask = (e) => {
    e.preventDefault();
    if (task.trim()) {
      setTasks([...tasks, task]);
      setTask(""); // Clear the input field
    }
  };

  // Function to remove a task from the list
  const removeTask = (index) => {
    const newTasks = tasks.filter((_, i) => i !== index);
    setTasks(newTasks);
  };

  return (
    <div
      style={{
        background: "linear-gradient(#e66465, #9198e5)",
        height: "100vh",
        display: "flex",
        justifyContent: "center",
        alignItems: "center",
      }}
    >
      <div
        style={{
          textAlign: "center",
          background: "white",
          width: "60%",
          height: "70%",
          borderRadius: "30px",
          padding: "20px",
          boxShadow: "0px 4px 12px rgba(0, 0, 0, 0.1)",
        }}
      >
        <h1>TODO List</h1>
        <form onSubmit={addTask} style={{ marginBottom: "20px" }}>
          <input
            type="text"
            value={task}
            onChange={(e) => setTask(e.target.value)}
            placeholder="Enter a task"
            style={{
              padding: "10px",
              width: "60%",
              borderRadius: "5px",
              border: "1px solid #ccc",
              marginRight: "10px",
              fontSize: "16px",
              boxShadow: "0px 2px 6px rgba(0, 0, 0, 0.1)",
            }}
          />
          <button
            type="submit"
            style={{
              padding: "10px 20px",
              borderRadius: "5px",
              border: "none",
              background: "#e66465",
              color: "white",
              fontSize: "16px",
              cursor: "pointer",
              boxShadow: "0px 2px 6px rgba(0, 0, 0, 0.1)",
            }}
          >
            Add
          </button>
        </form>
        <ul style={{ listStyleType: "none", padding: 0 }}>
          {tasks.map((task, index) => (
            <li
              key={index}
              style={{
                marginTop: "10px",
                fontSize: "18px",
                display: "flex",
                justifyContent: "center",
                alignItems: "center",
              }}
            >
              <span>{task}</span>
              <button
                onClick={() => removeTask(index)}
                style={{
                  marginLeft: "10px",
                  padding: "5px 10px",
                  borderRadius: "5px",
                  border: "none",
                  background: "#ff4d4d",
                  color: "white",
                  cursor: "pointer",
                  fontSize: "14px",
                }}
              >
                Remove
              </button>
            </li>
          ))}
        </ul>
      </div>
    </div>
  );
}

export default App;
```

---

## To-Do List

- [x] Launch portfolio at [devchanbin.vercel.app](https://devchanbin.vercel.app)
- [ ] Refactor and update the Roommate Matching Website Project
- [ ] Refactor the webreg project

---

## Resource
- [Resume PDF](/image/resume.pdf)