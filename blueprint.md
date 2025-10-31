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

### Current State (After Automated Deployment Setup)

*   **Infrastructure:**
    *   Configured for Firebase Hosting.
    *   `.firebaserc` file created to link to the `etqan-final` Firebase project.
    *   `firebase.json` file created to define the hosting configuration (public directory is set to the root folder).
*   **Automated Deployment (CI/CD):**
    *   **GitHub Actions Workflow:** A `.github/workflows/firebase-deploy.yml` file has been added to automate deployment.
    *   **Trigger:** The workflow is triggered on every push to the `main` branch.
    *   **Authentication:** The workflow uses Google Cloud's Workload Identity Federation to securely authenticate with Firebase without needing a long-lived service account key.
        *   A Workload Identity Pool (`github-pool`) and Provider (`github-provider`) have been created in the Google Cloud project.
        *   The `firebase-deployer` service account is configured to be impersonated by the GitHub Actions runner.
    *   **Deployment:** The workflow checks out the code and uses the `FirebaseExtended/action-hosting-deploy` action to deploy the website to Firebase Hosting.

## Current Plan

The website is now fully configured for automated deployments. Any changes pushed to the `main` branch on GitHub will be automatically deployed to the live Firebase Hosting URL: **https://etqan-6973c.web.app**

There are no further steps planned. The CI/CD pipeline is complete.
