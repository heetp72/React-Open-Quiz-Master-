# React Trivia App

This is a mini quiz application built with React that fetches trivia questions from the [Open Trivia Database](https://opentdb.com/). The app lets users enter their first name, choose a trivia category and difficulty level, and then answer a multiple-choice question. After submitting an answer, users receive immediate feedback on whether they were correct, along with the correct answer if needed.

## Features

- **Home Page Form Component**
  - Collects the user's first name.
  - Provides a dropdown to select a trivia category (Film, Mythology, Books, Television) using valid category IDs.
  - Provides a dropdown to choose the difficulty level (Easy, Medium, Hard).
  - Validates that all fields are filled before submission.
  - Displays error and success messages accordingly.
  - Fetches a trivia question from the Open Trivia Database API when the form is submitted successfully.

- **Question Form Component**
  - Displays the fetched trivia question.
  - Renders multiple-choice answers as radio buttons.
  - Validates that an answer is selected.
  - Provides feedback after submission with a green "Correct!" message or a red "Incorrect" message along with the correct answer.
  - Includes a "Start Over" button to reset the quiz and return to the home form.

- **State Management & Conditional Rendering**
  - Uses React state to manage form data, API responses, error/success messages, and the app's current step.
  - Conditionally renders either the Home Page or the Question Form based on user progress.

- **Styling with CSS Modules**
  - Implements component-specific styling using CSS modules in both the HomePage and the QuestionForm components.

## Technologies Used

- **React** – For building the user interface.
- **Vite** – For a fast development environment and bundling.
- **CSS Modules** – For component-scoped styling.
- **Open Trivia Database API** – For retrieving trivia questions.

## Usage

1. On the **Home Page**, enter your first name, select a category, and choose a difficulty level.
2. Click **Submit** to fetch a trivia question.
3. On the **Question Form**, read the question and select an answer by clicking the corresponding radio button.
4. Click **Submit Answer** to see if you were correct.
5. View the result message (green for correct, red for incorrect) and click **Start Over** to play again.
