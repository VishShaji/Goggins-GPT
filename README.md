# GogginsGPT Frontend

A React-based frontend for the GogginsGPT DSA tutor application.

## Deployment to AWS Amplify

1. Push your code to a Git repository (GitHub, GitLab, or BitBucket)

2. Set up AWS Amplify:
   - Go to AWS Amplify Console
   - Click "New App" > "Host Web App"
   - Connect to your Git provider and select your repository
   - Select the branch you want to deploy

3. Configure build settings:
   - The `amplify.yml` file is already configured for you
   - In the build settings, add the following environment variable:
     - Key: `REACT_APP_API_URL`
     - Value: Your backend API URL (e.g., https://your-api.amazonaws.com)

4. Click "Save and deploy"

## Environment Variables

- `REACT_APP_API_URL`: URL of the backend API
  - Local development: http://localhost:8003
  - Production: Your deployed backend URL

## Available Scripts

- `npm start`: Run the app in development mode
- `npm test`: Launch the test runner
- `npm run build`: Build the app for production
- `npm run eject`: Eject from create-react-app
