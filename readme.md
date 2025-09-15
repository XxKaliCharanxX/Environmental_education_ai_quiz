Welcome to EcoLearn! 🌍

Ever wanted to make a real impact on the planet while having some fun? EcoLearn is an interactive web app that turns environmental education into an exciting game. You can sign up, challenge your knowledge with endless AI-generated quizzes, watch your score grow, and climb the ranks on a global leaderboard.
✨ What You Can Do

    Join the Community: Create a secure account with our full sign-up and login system, complete with email verification to keep things safe.

    Never Stop Learning: Dive into dynamic quizzes powered by the Google Gemini API. You'll get fresh questions every single time you play!

    Grow at Your Own Pace: Our adaptive system adjusts the quiz difficulty for each topic based on how you're doing, creating a learning path that's just right for you.

    Earn Your Bragging Rights: Score points for every correct answer and watch your total climb. It’s all about learning and having fun.

    Become a Global Champion: See how you stack up against other eco-warriors on a live, real-time leaderboard, with a special podium for our top 3 players.

    Personalized User Dashboard & Profile: Users have a dedicated dashboard to see their stats at a glance and a profile page to view their details and rank.

    Serverless Backend: Utilizes Vercel Functions to securely handle API requests, keeping sensitive keys off the front-end.

    Fully Responsive Design: A clean, modern UI that works seamlessly across desktops, tablets, and mobile devices.

🛠️ Technology Stack

    Front-End: HTML5, CSS3, JavaScript (ES Modules)

    Backend as a Service (BaaS):

        Firebase Authentication: For user management.

        Firestore Database: For storing user profiles, points, and quiz progress.

    Serverless Functions: Vercel Functions

    AI Model: Google Gemini API

    Hosting: Vercel

🚀 Getting Started

Follow these instructions to set up and run the project locally or deploy it to your own Vercel account.
Prerequisites

    Node.js installed on your machine.

    A Google account for Firebase.

    A Google Gemini API Key.

    A Vercel account connected to your GitHub.

1. Firebase Project Setup

    Go to the Firebase Console and create a new project.

    Add a Web App to your project.

    Copy the firebaseConfig object provided. You will need this for all the HTML files.

    Enable Authentication -> Sign-in method -> Email/Password.

    Create a Firestore Database and start it in Test Mode for development.

2. Project Configuration

    Clone this repository to your local machine.

    Update Firebase Keys: In each of the HTML files (index.html, dashboard.html, challenges.html, quiz.html, leaderboard.html, profile.html), find the firebaseConfig object in the <script> tag and replace the placeholder values with the keys from your own Firebase project.

    Rename for Deployment: Rename registration.html to index.html. Vercel automatically uses index.html as the default landing page.

3. Deployment to Vercel

    Create a new repository on GitHub and upload your project files.

    Log in to Vercel and import your new GitHub repository.

    Configure Environment Variables: Before deploying, go to your project's Settings > Environment Variables. Add the following secret key:

        Key: GEMINI_API_KEY

        Value: Your_Secret_Gemini_API_Key

    Click Deploy. Vercel will automatically detect your vercel.json file and deploy the site along with the serverless function.

Your EcoLearn platform should now be live!