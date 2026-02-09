# vamcodeAutomationPractice
Para que practiques los comando de Git
# 🧪 UI & API Automation Challenge
## JavaScript / TypeScript – Cypress or Playwright

---

## General Requirements

- Use **JavaScript and/or TypeScript**
- Use **Cypress or Playwright** for UI automation
- Use **Node.js** and **npm**
- Use **Visual Studio Code** or **IntelliJ IDEA**
- Create a new project and add dependencies as needed
- Use a clean and scalable project structure
- Use a design pattern (Page Object Model or similar)
- Decide when to use hard assertions and soft assertions
- Browser must run maximized
- All paths and configurations must be relative so the project is portable
- All tests must be runnable with a single command

---

## UI Automation Challenge

### Application Under Test
https://www.saucedemo.com/

---

### Test Scenarios

#### 1. Login (Precondition)

Use the following credentials:

Username: standard_user  
Password: secret_sauce  

Validate that login is successful before executing other tests.

---

#### 2. Add Item to Shopping Cart

- Log in successfully
- Add any product to the shopping cart
- Validate:
  - Shopping cart icon counter increases
  - Product appears in the cart page

---

#### 3. Remove Item from Shopping Cart

- Add a product to the cart
- Navigate to the cart page
- Remove the product
- Validate:
  - Shopping cart is empty
  - Shopping cart icon counter is reset

---

#### 4. Product Validation (Search-like Behavior)

The application does not include a traditional search input.  
Validation must be performed against the product list on the inventory page.

Positive condition:
- Validate that the product "Sauce Labs Backpack" exists

Negative condition:
- Validate that the product "iPhone 15 Pro Max" does NOT exist

---

#### 5. Validate Store Information (Footer)

- Scroll down to the footer section
- Validate that store information text is displayed:
  - © 2024 Sauce Labs. All Rights Reserved.

---

## API Automation Challenge

### API Under Test
https://rickandmortyapi.com/documentation

---

### Test Scenarios

#### 6. Get Specific Character Information

Endpoint:
GET https://rickandmortyapi.com/api/character?name=Rick Sanchez

Validate:
- Response status code is 200
- Print only the following information in the console:

Character name: Rick Sanchez  
Status: Alive  

---

#### 7. Get All Characters and Map to TypeScript Model

Endpoint:
GET https://rickandmortyapi.com/api/character

Requirements:
- Map the response to a TypeScript interface or model
- Iterate through all characters
- Print the following output for each character:

Character name: Rick Sanchez  
Species: Human  
------------------------------------

Character name: Morty Smith  
Species: Human  
------------------------------------

---

## Final Delivery

- Use Page Object Model or equivalent
- Separate UI tests, API tests, page objects, models, and configuration files
- Ensure the project is fully portable
- Upload the completed project to Google Drive
- Share the access link via email
