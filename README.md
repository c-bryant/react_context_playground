# 🕹️ React Context API Playground

A dedicated reference architecture and educational sandbox demonstrating scalable global state management using React's native Context API and state hooks.

---

## 🛠️ Tech Stack & Patterns
* **Core Library:** React.js (Functional Components)
* **State Management:** React Context API, `useContext`, `useState`
* **Package Manager:** Yarn
* **Architecture Pattern:** Provider Pattern / Compound Components

---

## 🧠 Architectural Insights (For Mentees)

In modern React engineering, jumping straight into heavy external state libraries like Redux or Zustand is often overkill. This playground demonstrates how to leverage native React features to build a clean, scalable global data layer by focusing on three key concepts:

### 1. Encapsulation of Global Logic
Instead of instantiating context directly within UI views, this architecture wraps the initialization logic inside dedicated custom providers. UI components consume state via intuitive custom hooks (e.g., `useAppContext`), preventing components from needing to know the implementation details of the underlying state layer.

### 2. Mitigation of the "Prop-Drilling" Anti-Pattern
This project shows how to cleanly pass deep global variables (such as authentication states, application themes, or shared user data) down a complex component tree without manually passing props through intermediate layers that do not require the data.

### 3. Preventing Unnecessary Component Re-Renders
Mentees should study how context scopes are isolated here. By structuring localized consumer boundaries, we ensure that state updates only trigger a re-render in the exact components consuming the data, keeping the app optimized and performant.

---

## 💻 Local Setup & Execution

Run this project locally using Yarn:

1. **Clone the repository:**
   ```bash
   git clone
   
   ```

2. **Navigate into the project directory:**
   ```bash
   cd react_context_playground
   ```

3. **Install the dependencies:**
   ```bash
   yarn install
   ```

4. **Start the local development server:**
   ```bash
   yarn start
   ```
   Open [http://localhost:3000](http://localhost:3000) in your browser to view and interact with the state playground.
