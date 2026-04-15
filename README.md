# CI/CD Pipeline Demo

This is a simple demonstration of a CI/CD pipeline using GitHub Actions.

## Overview

This project contains a basic Node.js Express application with automated testing and deployment.

## Pipeline Features

- **Continuous Integration (CI)**: Runs on every push and pull request to the main branch
- **Automated Testing**: Runs unit tests using Jest
- **Multi-Node Testing**: Tests against Node.js versions 16.x and 18.x
- **Continuous Deployment (CD)**: Deploys to production on successful merge to main branch

## Project Structure

- `index.js`: Main application file
- `test.js`: Unit tests
- `package.json`: Dependencies and scripts
- `.github/workflows/ci.yml`: GitHub Actions workflow configuration

## How to Use

1. Push this code to a GitHub repository
2. The pipeline will automatically run on pushes to the main branch
3. Check the Actions tab in GitHub to see the pipeline execution

## Local Development

```bash
npm install
npm test
npm start
```

## Pipeline Stages

1. **Test Job**:
   - Installs dependencies
   - Runs tests across multiple Node.js versions
   - Builds the application

2. **Deploy Job**:
   - Runs only on successful tests and pushes to main
   - Simulates deployment (in a real scenario, this would deploy to a server/cloud)