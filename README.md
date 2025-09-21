# KalaSaarthi - An AI-Powered Artisan Marketplace
KalaSaarthi is a modern, responsive e-commerce platform designed to connect local Indian artisans directly with buyers. The platform empowers sellers by using the Google Gemini API to automatically generate compelling product titles, descriptions, and tags, simplifying the process of listing handmade goods.


A preview of the KalaSaarthi marketplace interface.

## Key Features

### For Buyers:
Intuitive Marketplace: Browse a beautiful grid of unique, handmade products.

Advanced Filtering & Sorting: Easily find items by category, color, price range, and newest arrivals.

Voice Search: Search for products using voice commands for a hands-free experience.

Detailed Product View: View multiple product images, read detailed descriptions, and see pricing.

Shopping Cart: Add and remove items from your cart before checkout.

Secure Checkout: Place orders and have them recorded in your dashboard.

User Dashboard: View past orders, manage your shipping address, and see your wishlist.

Dark & Light Mode: Switch between themes for comfortable viewing.

### For Artisans (Sellers):
AI-Powered Listing Creation: A simple, three-step process to list a new product:

Upload Photos: Add images of your craft.

Share Your Story: Write a brief story or description of your product and its inspiration.

AI Generation & Review: The Google Gemini API automatically generates a professional title, a detailed e-commerce description, relevant tags, and a suggested price based on your story. You can review and edit before publishing.

Seller Dashboard: Get an overview of your listed products and their status (available/sold).

Product Management: Mark items as "sold," "available," or delete listings entirely.

Sales Analytics: (Future Scope) A dashboard to visualize sales data and performance.

## Technology Stack
Frontend: HTML5, CSS3, Vanilla JavaScript (ES6 Modules)

Styling: Tailwind CSS for a utility-first design system.

Backend & Database: Firebase

Authentication: User sign-up and sign-in (Email/Password).

Firestore: NoSQL database for storing user, product, and order data in real-time.

Hosting: Deployed live on the web with Firebase Hosting.

Generative AI: Google Gemini API for automated product content generation.

## Getting Started
Follow these instructions to get a local copy up and running for development and testing purposes.

Prerequisites
A Google account to create a Firebase project.

Node.js installed on your machine (for the Firebase CLI).

Installation & Setup
Clone the repository:

git clone [https://github.com/GUGHAN-3001/kalasaarthi.git](https://github.com/GUGHAN-3001/kalasaarthi.git)
cd kalasaarthi

Set up Firebase:

Go to the Firebase Console and create a new project.

In your new project, go to Project Settings > General.

Under "Your apps," click the Web icon (</>) to register a new web app.

Copy the firebaseConfig object. You will need to paste this into index.html.

In the Firebase Console, go to Build > Authentication and enable the Email/Password sign-in provider.

Go to Build > Firestore Database and create a database in production mode.

Set up Gemini API Key:

Go to Google AI Studio to get your free API key.

Open index.html and paste your API key into the GEMINI_API_KEY constant at the top of the <script> tag.

Install Firebase CLI and Run Locally:

# Install the Firebase command-line tools
npm install -g firebase-tools

# Log in to your Google account
firebase login

# Test the app on a local server
firebase serve

Your application should now be running on http://localhost:5000.

## Deployment
To deploy the application to the web, use the Firebase CLI.

Initialize Firebase in your project directory (one-time setup):

firebase init hosting

Select Use an existing project and choose your Firebase project.

Use . as your public directory.

Answer No to the single-page app question.

Deploy to Firebase Hosting:

firebase deploy --only hosting

After deployment, the CLI will provide you with the live URL for your project.
