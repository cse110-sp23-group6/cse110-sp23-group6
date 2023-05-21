# SixthSense Project - CI/CD Pipeline Phase 1 Status

## Current Functionalities

### Code Style and Linting Enforcement

- We have a Style Guide set up which every team member uses and appropriate CSS/Style properties to maintain consistency across all the pages in the webpages.
  
- We may plan to integrate a linter into our development environment, which helps enforce coding standards and maintain consistent code style.
  - Mostly after everyone has completed working on HTML and CSS components of all pages and merges to Main.

- Potentially, a linter will run locally in all our editors
  providing real-time feedback on code style violations.
    
### Code Quality via Tools
- We have set up Codeclimate as our code quality analysis tool.
- Codeclimate analyzes our codebase and provides insights into potential issues, such as complexity, duplication, and maintainability.
- The tool generates automated code quality reports, allowing us to identify areas that need improvement.

### Code Quality via Human Review
- We have implemented a pull request (PR) workflow using our version control system (e.g., Git).
  
- Pull requests serve as a mechanism for code review, where team members review each other's code changes.

- Most of the Pull Requests will be reviewed and merged to main in the weekly meetings to thoroughly check the progress and merge only if it matches the issue requirements.
  
- Through this process, we ensure code quality, catch bugs, and share knowledge among the team.

### Unit Tests via Automation
- We have selected Jest as our unit testing framework.
  
- Unit tests will be written and automated using Jest, ensuring that individual components and functions are tested for correctness.

- The tests cover critical functionality and help identify regressions as the codebase evolves.

- At this stage, there is not much testing as the webpages are not linked yet. In the next sprint, we'll be testing as we go along to check critical functionalites.

### Documentation Generation via Automation
- We are utilizing JSDoc to generate automated documentation for our codebase.
- Example of a convention ->
  
```/**
 * Adds two numbers.
 * @param {number} a - The first number.
 * @param {number} b - The second number.
 * @returns {number} The sum of the two numbers.
 */
function addNumbers(a, b) {
  return a + b;
}
```

- By following JSDoc conventions, we can document our code, including functions, classes, and modules, and generate HTML-based documentation automatically.


--- 


## Planned/In-Progress Enhancements

### Integration Tests

- We are currently planning to introduce integration tests to validate the interaction between different components and ensure smooth integration of UI/UX pages.

### Continuous Integration Setup

- We intend to set up a CI server (such as Jenkins) to automate the build and test process triggered by code changes.


### Deployment Automation
- We are exploring deployment automation options to streamline the deployment process of our completed CSS and HTML parts of each page.

## CI/CD Pipeline Diagram

Please find below the diagram representing our current CI/CD pipeline setup:

[CI/CD Pipeline Diagram](https://github.com/cse110-sp23-group6/cse110-sp23-group6/blob/main/admin/cipipeline/phase1.png)

