# New App

## Overview

New App is a user-friendly application that allows users to create, save, and manage jokes. It incorporates modern technologies like SolidJS, Tailwind CSS, and Vite for a smooth and responsive user experience. The app also integrates with Supabase for authentication and utilizes various AI-powered features through event handling.

## User Journeys

### 1. Sign In with ZAPT

1. Upon opening the app, the user is presented with a login screen titled "Sign in with ZAPT".
2. The user can learn more about ZAPT by clicking the link, which opens `https://www.zapt.ai` in a new tab.
3. The user signs in using one of the available providers: Email (Magic Link), Google, Facebook, or Apple.
4. Upon successful authentication, the user is redirected to the Home Page.

### 2. Home Page Features

#### a. Adding a New Joke Manually

1. On the Home Page, the user sees a form to add a new joke with "Setup" and "Punchline" fields.
2. The user inputs their joke and clicks "Save Joke".
3. The joke is saved, and it appears in the "Joke List" section.

#### b. Generating a Joke with AI

1. The user clicks the "Generate Joke" button.
2. The app shows a loading state while fetching a joke from the AI.
3. The generated joke appears in the input fields.
4. The user can edit the joke if desired and click "Save Joke" to add it to their list.

#### c. Viewing the Joke List

1. The "Joke List" displays the user's saved jokes in a scrollable section.
2. Each joke shows the setup in bold and the punchline below it.

#### d. Additional Features

##### i. Generate Image

1. The user clicks "Generate Image".
2. The app shows a loading state while generating an image based on a prompt.
3. The generated image appears below, displaying a funny cartoon character telling a joke.

##### ii. Text to Speech

1. If a joke is present in the input fields, the user can click "Text to Speech".
2. The app converts the joke into an audio file.
3. An audio player appears, allowing the user to listen to the joke.

##### iii. Generate Markdown Story

1. The user clicks "Generate Markdown".
2. The app generates a short, funny story about a comedian in markdown format.
3. The story is rendered below with proper formatting.

### 3. Sign Out

1. At any time, the user can click the "Sign Out" button at the top right.
2. The user is logged out and returned to the login screen.

## External APIs and Services

- **Supabase Authentication**: Used for user authentication via email magic links and social providers.
- **ZAPT AI Events**: Handles AI-powered features such as joke generation, image generation, text-to-speech conversion, and markdown story creation.
- **Sentry Error Logging**: Integrated to log errors on both frontend and backend for better debugging and monitoring.

## Technologies Used

- **SolidJS**: For building reactive user interfaces.
- **Tailwind CSS**: For styling and responsive design.
- **Vite**: As the build tool for faster development.
- **Supabase Auth UI**: Provides pre-built authentication components.
- **Sentry**: For error tracking and logging.
