# Strapi Learning Assignment

## Overview
This assignment involves learning and working with Strapi, an open-source headless CMS, as part of the internship at Tangence. The goal is to understand the basics of Strapi, set up a project, and create and manage content types and APIs.

## Table of Contents
- [Project Setup](#project-setup)
- [Creating Content Types](#creating-content-types)
- [Managing Content](#managing-content)
- [Using the API](#using-the-api)
- [Deployment](#deployment)
- [Resources](#resources)

## Project Setup
1. **Install Node.js and npm**: Ensure you have Node.js (v12 or higher) and npm installed on your machine. You can download them from [Node.js official website](https://nodejs.org/).

2. **Install Strapi**:
    ```bash
    npx create-strapi-app my-project --quickstart
    ```

3. **Run Strapi**:
    ```bash
    cd my-project
    npm run develop
    ```

4. **Access Strapi Admin**: Open your browser and go to `http://localhost:1337/admin`. Follow the instructions to create an admin user.

## Creating Content Types
1. **Navigate to Content-Type Builder**: In the Strapi admin panel, go to the "Content-Type Builder".

2. **Create a New Content Type**:
    - Click on the "Create new collection type" button.
    - Name your content type (e.g., `Article`).
    - Add fields to your content type (e.g., title, body, author).

3. **Save and Restart**: Save your new content type and restart the server if necessary.

## Managing Content
1. **Add Content**:
    - Navigate to the "Content Manager" in the Strapi admin panel.
    - Select the content type you created (e.g., `Article`).
    - Click on "Create new entry" and fill in the fields.

2. **Publish Content**: Once you are done filling out the fields, click on "Save" and then "Publish".

## Using the API
1. **Fetch Content**:
    - Use the following endpoint to fetch published content:
        ```bash
        GET http://localhost:1337/articles
        ```
    - You can use tools like Postman or cURL to test the API.

2. **Fetch Single Content Item**:
    - Use the following endpoint to fetch a single content item by its ID:
        ```bash
        GET http://localhost:1337/articles/:id
        ```

