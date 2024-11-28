<div align="center">
  <img src="./frontend/omnigpt/src/assets/images/logos/logo-no-background.svg" alt="ClickClick Logo" width=150 height=150>
</div>

# OmniGPT

**Uniting Every Perspective, Amplifying Every Insight**

Welcome to **OmniGPT**, your one-stop platform for accessing multiple GPT models in a single app. Whether you're crafting content, developing code, or conducting research, OmniGPT empowers you to compare and select the best responses for your needs. Experience unparalleled flexibility, enhance your work's quality, and save on costs with our affordable subscription plans. Discover the power of multiple GPTs at your fingertips. Sign up today!

## Deployed
[![Netlify Status](https://api.netlify.com/api/v1/badges/9e4915f9-eaea-45f9-b2b7-64fca4a26198/deploy-status)](https://app.netlify.com/sites/omnigpt-geeks/deploys)
Access OmniGPT Here ⮕ [OmniGPT](https://omnigpt-geeks.netlify.app/)

<h2 align="center">💻 Tech Stack</h2>
<p align="center">
    <img alt="React" src="https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB"/>
    <img alt="TailwindCSS" src="https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white">
    <img alt="NPM" src="https://img.shields.io/badge/NPM-%23CB3837.svg?style=for-the-badge&logo=npm&logoColor=white">
    <img alt="AWS Lambda" src="https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white">
    <img alt="Firebase" src="https://img.shields.io/badge/firebase-%23039BE5.svg?style=for-the-badge&logo=firebase">
    <img alt="Netlify" src="https://img.shields.io/badge/netlify-%23000000.svg?style=for-the-badge&logo=netlify&logoColor=#00C7B7">
    <img alt="VITE" src="https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white">
</p>

## Everything You Need

### Multi-GPT Access
Access responses from multiple GPT models for a single prompt, ensuring diverse perspectives and comprehensive insights.

### Response Comparison
Compare and choose the best response from different GPT models based on performance and relevance to your needs.

### Affordable Subscription Plans
Enjoy cost-effective subscription plans that make multi-GPT access affordable for individuals and small businesses.

### Exclusive Partnerships
Benefit from exclusive partnerships with diverse GPT model providers, offering a unique and extensive range of model responses.

### Developer-Friendly Features
Tools and integrations designed for developers to enhance productivity and streamline coding tasks with the help of multiple GPT responses.

### Comprehensive Support
Access to dedicated customer support to resolve issues promptly and ensure a smooth user experience.

## Experimental Features

### Stripe Payment (Experimental)
Our Stripe payment feature is currently under development. To try it out, create a Stripe account and replace Stripe keys in `backend/Stripe/controller/subscriptionController.js` along with `firebaseSDK.json`.

## Features

### Landing Page
Discover OmniGPT and its offerings with an engaging and informative landing page.
[Explore the Landing Page](https://omnigpt-geeks.netlify.app/)

### Login
Secure and user-friendly login system to access your OmniGPT account.
[Login to OmniGPT](https://omnigpt-geeks.netlify.app/login)

### Registration
Easy registration process to join our platform and start your subscription.
[Register on OmniGPT](https://omnigpt-geeks.netlify.app/register)

### Pricing
Transparent and flexible pricing options tailored to different user needs.
[View Pricing Plans](https://omnigpt-geeks.netlify.app/pricing)

## Running the Frontend

Follow these steps to set up and run the frontend of OmniGPT:

### Prerequisites

Make sure you have the following installed on your machine:
- **Node.js** (version 14.x or later)
- **npm** (version 6.x or later)
- **Firebase** (Create a project and setup authentication)

### Installation

1. **Clone the Repository**

    ```bash
    git clone https://github.com/yourusername/omni-gpt.git
    ```

2. **Navigate to the Project Directory**

    ```bash
    cd csci5193-geeksquad-omnigpt/frontend/omnigpt/
    ```

3. **Create an `.env` File**

    In the root directory, create an `.env` file and add the following variables with their corresponding values:

    ```plaintext
    VITE_GEMINI_KEY = [Your Gemini Key]
    VITE_LLAMA_API_ENDPOINT = [Your Llama API Endpoint]

    VITE_FIREBASE_API_KEY = [Your Firebase API Key]
    VITE_FIREBASE_AUTH_DOMAIN = [Your Firebase Auth Domain]
    VITE_FIREBASE_PROJECT_ID = [Your Firebase Project ID]
    VITE_FIREBASE_STORAGE_BUCKET = [Your Firebase Storage Bucket]
    VITE_FIREBASE_MESSAGING_SENDER_ID = [Your Firebase Messaging Sender ID]
    VITE_FIREBASE_APP_ID = [Your Firebase App ID]
    VITE_FIREBASE_MEASUREMENT_ID = [Your Firebase Measurement ID]
    ```

4. **Set up the Llama API Endpoint**

    - Deploy a Lambda function with files from `backend/Llama`.
    - Update the API key in `index.mjs` following the guide at [Meta Llama Documentation](https://replicate.com/meta/meta-llama-3.1-405b-instruct).

5. **Firebase Setup**

    Create a Firebase project and update the Firebase-related environment variables in the `.env` file.

6. **Obtain a Gemini API Key**

    Register and get your Gemini key from [Google's Gemini API Documentation](https://ai.google.dev/gemini-api/docs/api-key).

7. **Install Dependencies**

    ```bash
    npm install
    ```

8. **Start the Server**

    ```bash
    npm start
    ```

### Building for Production

To build the project for production, use:

```bash
npm run dev
