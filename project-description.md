# Test Project Outline – Module D – Interactive Guest Experience

## Competition time

4 hours

## Introduction

Developers will focus on creating an interactive frontend application for guests utilizing the DineEase service. This project challenges students to build a modern Single Page Application (SPA) using a JavaScript framework that provides users with an intuitive platform to explore restaurants, view detailed menus, read past reviews, and place orders. The application emphasizes user experience, proper authentication handling, and seamless integration with backend APIs.

## General Description of Project and Tasks

The project requires building a complete frontend guest experience application with the following key components:

- **Pages**: 4 main pages (Login, Registration, Restaurant Browse/Homepage, Restaurant Detail with Menu, Finish Order)
- **Technology**: Modern JavaScript framework (React, Vue.js, or Angular) with SPA architecture
- **Authentication**: JWT-based user authentication with proper token management
- **Features**: User login/registration, restaurant browsing with search, menu display, cart management, order placement, and review system
- **User Experience**: Responsive design, proper error handling, form validation, and persistent cart functionality
- **Integration**: Backend API integration for authentication, restaurant data, ordering, and reviews

Students must demonstrate proficiency in frontend development, state management, API integration, and creating polished user interfaces suitable for a commercial restaurant platform.

## Requirements

The goal of the application is to provide DineEase restaurant service guests with a comprehensive digital platform for discovering restaurants, viewing menus, placing orders, and sharing reviews. Users must be able to create accounts, authenticate securely, browse restaurant options, manage their orders, and provide feedback through an intuitive and responsive web interface.

The application should simulate a real-world restaurant discovery and ordering platform, emphasizing user experience, security, and functionality. All features must work seamlessly together to create a cohesive guest experience.

The following pages and functionality must be implemented:

### 1. User Login Page

Developers need to create a dedicated login page where users can enter their credentials and gain access to the platform. The login process will be facilitated by the provided backend API.

#### **Login**

- **Objective:** Allow users to log in using their registered email and password.
- **UI Elements:**
  - Email Input Field
  - Password Input Field
  - Login Button
  - Link to the Registration Page for new users
- **Functional Requirements:**
  - Input validation for correct email format.
  - Masked password input.
  - Error handling for failed login attempts.
  - On successful login, store the received JWT token for authenticating subsequent requests.

#### **Logout**

- **Objective:** Offer users a mechanism to securely log out from their session.
- **UI Elements:**
  - Logout Button
- **Functional Requirements:**
  - Clear the stored JWT token.
  - Redirect the user back to the login page.

### 2. New User Registration Page

A platform for new users to sign up and create an account.

- **Objective:** Enable users to create a new account by providing their email, password, and name.
- **UI Elements:**
  - Name Input Field
  - Email Input Field
  - Password Input Field
  - Confirm Password Input Field
  - Registration Button
  - Back to Login Button
- **Functional Requirements:**
  - Input validation for correct email format and password matching.
  - After successful registration, store the received JWT token and direct the user to the homepage.
  - Provide feedback in case of errors, like when an email is already registered.

### 3. Browsing and Searching Restaurants Page (homepage)

Facilitate users in exploring and searching for restaurants.

- **Objective:** Display a list of restaurants and offer a search functionality.
- **UI Elements:**
  - Search Bar
  - Tile view of restaurants with name, description, average rating and "Continue" link.
  - "Show more results" link
- **Functional Requirements:**
  - Fetch and display restaurants from the backend.
  - Display 6 randomly selected restaurants at first time. If there are more restaurants and user clicks on the "Show more results" link, all the remained restaurants should appear.
  - Implement search functionality by making requests to the backend with the query string. Display the first 6 from restaurants from the search results, and use the "Show more results" as above.
  - Clicking on Continue link of a restaurant card will redirect the user to the detailed restaurant page.
  - Restaurants that the user has previously ordered from are displayed with a purple border.

### 4. Restaurant Page with Menu Card

A dedicated page showcasing all details related to a selected restaurant.

#### **Ordering**

- **Objective:** Allow users to select dishes from the menu and place an order.
- **UI Elements:**
  - List of menu items with name and price.
  - Quantity selector for each menu item.
  - Add to cart (+) button.
  - Finish Order button.
- **Functional Requirements:**
  - If users click the "Add to Cart" button next to a menu item, that item will be added to the cart with a quantity of 1.
  - The "Finish Order" button displays the total amount of the order.
  - Clicking finish order button Finish Order page should appear.
  - Orders should be retained when the browser is reloaded.

#### **Review with Rating**

- **Objective:** Users should be able to leave reviews and ratings for a restaurant.
- **UI Elements:**
  - Star Rating Selector (1-5 stars).
  - Comment Text Area.
  - Submit Review Button.
  - List of past reviews with reviewer name, rating, and comment.
- **Functional Requirements:**
  - Submitting a review sends the rating and comment to the backend.
  - Fetch and display past reviews for the restaurant from the backend.

### _Finish Order_

#### **Objective:**

Facilitate the user in finalizing their order, making payment, and receiving a confirmation.

#### **UI Elements:**

- **Review Cart:** A summary of all items added with their respective quantities and individual prices.
- **Total Amount:** Displays the cumulative price of all items.
- **Finish Order Button:** To finalize the order after verifying all details.

#### **Functional Requirements:**

- Upon selecting items and clicking the "Finish Order" button, the user should be shown their cart's content.
- Users should have the ability to remove items.
- Display an estimated total.
- Post-confirmation, the user should receive an on-screen message.

## Assessment

The project will be assessed using multiple evaluation methods to ensure comprehensive coverage of both technical implementation and user experience aspects:

**Technical Assessment:**
- Code review for JavaScript framework usage, component structure, and best practices
- Functionality testing across different browsers and devices
- API integration verification and error handling evaluation
- Authentication and security implementation review

**User Experience Evaluation:**
- Interface design and usability testing
- Responsive behavior across mobile, tablet, and desktop viewports
- Form validation and error messaging assessment
- Overall user flow and navigation evaluation

**Assessment Tools:**
- Modern web browsers (Chrome, Firefox, Safari, Edge) for cross-browser testing
- Browser developer tools for responsive design and performance analysis
- Manual testing of all user workflows and edge cases
- Code quality assessment using industry standards and best practices

## Mark distribution

| WSOS SECTION | Description                            | Points |
|--------------|----------------------------------------|--------|
| 1            | Work organization and self-management  | 0      |
| 2            | Communication and interpersonal skills | 0      |
| 3            | Design Implementation                  | 4.5    |
| 4            | Front-End Development                  | 15.5   |
| 5            | Back-End Development                   | 0      |
| **Total**    |                                        | **20** |
