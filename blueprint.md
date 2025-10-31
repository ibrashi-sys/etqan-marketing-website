# Etqan Marketing Website - Blueprint

## Overview

A modern, responsive, single-page marketing website for "Etqan for Research and Marketing". The site is focused on industrial clients, highlighting services like Overall Equipment Effectiveness (OEE) analysis, marketing strategy, and business leadership. It is built with HTML and Tailwind CSS and is designed to be deployed on Firebase Hosting.

## Project Documentation

### Initial Version

*   **Design & Style:**
    *   Modern, clean, and professional design.
    *   Uses Tailwind CSS for utility-first styling.
    *   Primary color: Teal.
    *   Responsive layout for mobile and desktop.
    *   Sticky header/navigation.
    *   Visually appealing hero section with a strong call to action.
    *   Features section with icons and descriptions.
    *   Contact form.
    *   Footer with social media links.
*   **Features:**
    *   Single-page application structure.
    *   Navigation links scroll to different sections of the page (`#features`, `#contact`).
    *   The "Customer Platform" button is a placeholder.
    *   The hero section includes a placeholder image for a dashboard screenshot.
    *   The features are tailored to an industrial audience:
        1.  Production Efficiency Analysis (OEE).
        2.  Industrial Marketing and Global Expansion.
        3.  Business Leadership and Strategic Development.
    *   A simple contact form is included.

### Current State (After Firebase Setup)

*   **Infrastructure:**
    *   Configured for Firebase Hosting.
    *   `.firebaserc` file created to link to the `etqan-final` Firebase project.
    *   `firebase.json` file created to define the hosting configuration (public directory is set to the root folder).

## Current Plan

**Goal:** Manually deploy the website to Firebase Hosting.

**Steps:**
The user has requested to perform the deployment steps manually. The following commands will be provided to the user.

1.  **Install Firebase CLI:**
    ```bash
    npm install -g firebase-tools
    ```
2.  **Login to Firebase:**
    ```bash
    firebase login
    ```
3.  **Deploy the site:**
    ```bash
    firebase deploy --only hosting
    ```
