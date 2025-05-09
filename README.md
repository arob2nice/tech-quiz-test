# Tech Quiz Testing Suite

## Description

This project is a **Tech Quiz application** built with the MERN stack (MongoDB, Express.js, React, Node.js). It allows users to take a 10-question quiz and view their final score. The objective of this challenge was to implement **comprehensive testing** using **Cypress** for both **component** and **end-to-end (E2E)** functionality, ensuring the reliability and performance of the application.

## Table of Contents

- [User Story](#user-story)  
- [Acceptance Criteria](#acceptance-criteria)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Tests](#tests)  
- [Folder Structure](#folder-structure)  
- [Walkthrough Video](#walkthrough-video)  
- [Credits](#credits)  
- [License](#license)

## User Story

```md
AS AN aspiring developer  
I WANT to take a tech quiz  
SO THAT I can test my knowledge and improve my skills  
```

## Acceptance Criteria

```md
GIVEN I am taking a tech quiz  
WHEN I click the start button  
THEN the quiz starts and I am presented with a question  
WHEN I answer a question  
THEN I am presented with another question  
WHEN all questions are answered  
THEN the quiz is over  
WHEN the quiz is over  
THEN I can view my score  
WHEN the quiz is over  
THEN I can start a new quiz  
```

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/arob2nice/tech-quiz-test.git
   cd tech-quiz-test
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Install Cypress as a dev dependency:
   ```bash
   npm install --save-dev cypress
   ```

4. Rename `.env.example` to `.env` and provide the necessary environment variables.

## Usage

To start the app locally:

```bash
npm run develop
```

To run all Cypress tests:

```bash
npm run test
```

This will run both component and end-to-end test suites.

## Tests

The application is tested using [Cypress](https://docs.cypress.io):

- **Component Test** (`cypress/component/Quiz.cy.jsx`)
  - Renders the quiz component and validates UI elements.
  
- **End-to-End Test** (`cypress/e2e/quiz.cy.js`)
  - Tests full quiz flow: start quiz, answer questions, view score, restart quiz.

## Folder Structure

```md
.
├── client/                 # React frontend
├── server/                 # Node.js/Express backend
├── cypress/               
│   ├── component/          # Component tests
│   │   └── Quiz.cy.jsx     
│   ├── e2e/                # End-to-end tests
│   │   └── quiz.cy.js      
│   ├── fixtures/           # Mock data for testing
│   │   └── questions.json  
│   └── tsconfig.json       
├── .gitignore
├── cypress.config.ts
├── package.json
├── tsconfig.json
└── README.md
```

## Walkthrough Video

📽️ [Watch the walkthrough video here](https://drive.google.com/file/d/139ZiOxWU0olSavse9RT0EvTwgGo8UzSd/view)  
The video includes:
- Running all tests from the command line
- Component test execution
- End-to-end quiz flow test
- Confirmation that all tests pass

## GitHub Repository

🔗 [https://github.com/arob2nice/tech-quiz-test](https://github.com/arob2nice/tech-quiz-test)

## Credits

Project bootstrapped from a full-stack Tech Quiz app provided by the GW Coding Bootcamp.

## License

This project is licensed under the [MIT License](LICENSE).
