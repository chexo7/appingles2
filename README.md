# English Grammar Quiz

An interactive quiz application built with React, TypeScript, Vite, and the Google Gemini API. It's designed to help B1-B2 level Spanish speakers practice English grammar in a fun and engaging way.

## Features

-   **Infinite Questions:** Practice as long as you want with an endless stream of grammar questions.
-   **Intelligent Pre-fetching:** The next question is loaded in the background for an instant, seamless transition.
-   **Detailed Feedback:** Get instant corrections with clear, simple explanations in Chilean Spanish when you make a mistake.
-   **User-Controlled Pace:** A "Next Question" button appears on incorrect answers, allowing you to learn at your own pace.
-   **Responsive Design:** Looks great on both desktop and mobile devices.

## Tech Stack

-   **Framework:** React 19 with TypeScript
-   **Build Tool:** Vite
-   **Styling:** Tailwind CSS
-   **AI:** Google Gemini API (`gemini-2.5-flash-preview-04-17`)

---

## Local Development

**1. Prerequisites:**
   - [Node.js](https://nodejs.org/) (version 18 or newer recommended)
   - A code editor like [VS Code](https://code.visualstudio.com/)

**2. Get an API Key:**
   - You need a Google Gemini API key. You can get one from [Google AI Studio](https://aistudio.google.com/app/apikey).

**3. Setup:**
   - Clone the repository.
   - Create a file named `.env.local` in the root of the project.
   - Add your API key to the `.env.local` file like this:
     ```
     VITE_GEMINI_API_KEY=TU_API_KEY_AQUI
     ```
   - Open your terminal, navigate to the project directory, and install the dependencies:
     ```bash
     npm install
     ```
   - Start the development server:
     ```bash
     npm run dev
     ```
   - Open your browser and go to `http://localhost:5173` (or the address shown in your terminal).

---

## Deployment to Vercel (Recommended)

You can deploy this application with zero configuration on Vercel.

**1. Push to GitHub:**
   - Create a new repository on [GitHub](https://github.com/new).
   - Upload all the files from this project to your new repository.

**2. Deploy on Vercel:**
   - Sign up or log in to [Vercel](https://vercel.com/).
   - Click "Add New..." -> "Project".
   - Import your GitHub repository.
   - **Crucial Step:** Before deploying, go to the "Environment Variables" section.
     - Add a new variable:
       - **Name:** `VITE_GEMINI_API_KEY`
       - **Value:** Paste your Gemini API key here.
   - Click "Deploy". Vercel will automatically detect that this is a Vite project, build it, and deploy it.
