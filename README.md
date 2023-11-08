# React Timer Challenge

This repository contains two React components that work together to create a timer-based challenge and display the result in a modal dialog. The two components are:

1. `TimerChallenge`: A component that allows you to set a target time, start a timer, and track the time remaining. When the timer reaches zero, it opens a modal dialog to show the result.

2. `ResultModal`: A modal dialog component that displays the result of the timer challenge, including the user's score and the remaining time.

## Getting Started

Follow these instructions to get the Timer Challenge and ResultModal components up and running in your React project.

### Prerequisites

Before using these components, make sure you have the following dependencies installed in your React project:

- React: You should have React set up in your project.

### Installation

1. Install the Timer Challenge and ResultModal components by importing them into your project.

   ```javascript
   import TimerChallenge from './TimerChallenge';
   import ResultModal from './ResultModal';
   ```

2. Use the `TimerChallenge` component in your JSX code by passing the required props:

   ```javascript
   <TimerChallenge title="Your Challenge Title" targetTime={60} />
   ```

3. The `ResultModal` component is used internally by the `TimerChallenge` component and does not need to be used separately.

### `TimerChallenge` Props

- `title` (String): The title of the challenge.
- `targetTime` (Number): The target time for the challenge in seconds.

### Functions

- `handleStart()`: Start the timer when the "Start Challenge" button is clicked.
- `handleStop()`: Stop the timer and open a result modal when the "Stop" button is clicked.
- `handleReset()`: Reset the timer to the initial target time.

### Usage

To use the `TimerChallenge` component, you need to import it and pass the necessary props as shown in the Installation section. The component will render with the provided title and target time.

Click the "Start Challenge" button to begin the timer. The timer will count down from the target time. When the timer reaches zero, a modal dialog will open, showing the result.

You can also click the "Stop" button to stop the timer and open the result modal prematurely.

### `ResultModal` Props

- `targetTime` (Number): The target time for the challenge in seconds.
- `remainingTime` (Number): The remaining time on the timer.
- `onReset` (Function): A callback function to reset the challenge.

### Example

Here's an example of how to use the `TimerChallenge` component in your React application:

```javascript
import React from 'react';
import TimerChallenge from './TimerChallenge';

function App() {
  return (
    <div className="App">
      <TimerChallenge title="Coding Challenge" targetTime={120} />
    </div>
}

export default App;
```

## Acknowledgments

- This component set was created as a simple timer challenge tool for React applications.
- Inspired by coding challenges and productivity apps.
 
![image](https://github.com/akifalbayrak/Countdown/assets/142679378/9bf85f4f-1294-44c6-9aa9-aec55984049f)
