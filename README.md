# SauceDemo Cypress Automation

This project contains end-to-end test automation for the [SauceDemo](https://www.saucedemo.com/) web application using Cypress.  
It covers functional, regression, and negative test scenarios including login, inventory management, cart, and checkout workflows.

---

## Project Overview

- **Application Under Test (AUT):** [https://www.saucedemo.com/](https://www.saucedemo.com/)
- **Framework:** Cypress (JavaScript)
- **Modules Covered:**
  - Login
  - Inventory
  - Cart
  - Checkout
  - Menu (Side Navigation)
  - Negative & Edge Cases
  - UI/UX Validation

---

## Folder Structure

```

saucedemo-cypress/
│
├── cypress/
│   ├── e2e/            # Test specs (by module)
│   ├── fixtures/       # Test data (e.g., credentials.json)
│   ├── support/        # Custom commands & Page Objects
│
├── node\_modules/       # Dependencies
├── cypress.config.js   # Cypress configuration
├── package.json        # Project dependencies & scripts
└── README.md           # Project documentation

```

---

## Installation & Setup

1. Clone this repository:

   ```bash
   git clone https://github.com/siddhugurubhetti8483/saucedemo-cypress.git

   cd saucedemo-cypress
   ```

2. Create Json Package

   ```bash
   npm init -y
   ```

3. Install Cypress for fresh project:

   ```bash
   npm install cypress --save-dev
   ```

4. Install dependencies after clone:

   ```bash
   npm install cypress --save-dev
   ```

5. Run tests in headed mode:

   ```bash
   npx cypress open
   ```

6. Run tests in headless mode:

   ```bash
   npx cypress run
   ```

---

## Test Coverage

### **1. Login Tests**

- Valid login with standard_user
- Invalid login (wrong username/password)
- Locked_out_user login
- Empty username/password validation
- Case sensitivity checks

### **2. Inventory Page Tests**

- Verify product list (6 items)
- Product details: name, price, image
- Sorting functionality (A-Z, Z-A, Price low-high, high-low)
- Add to Cart / Remove functionality
- Cart badge updates
- Navigate to product detail page

### **3. Cart Tests**

- Verify added products
- Remove products
- Continue shopping navigation
- Checkout button navigation

### **4. Checkout Tests**

- Step One: form validations
- Step Two: overview validations (items, totals, tax, grand total)
- Order completion & confirmation

### **5. Menu Tests**

- Open/close menu
- Logout functionality
- Reset App State (cart reset)

### **6. Negative & Edge Cases**

- Checkout with empty cart
- Direct URL access without login
- Session persistence after refresh
- Access after logout (back button behavior)

### **7. UI/UX Validations**

- Header, footer, and logo visibility
- Button states and alignment
- Responsive checks (different viewports)

---

## Future Enhancements

- Integration with CI/CD (GitHub Actions, Jenkins)
- Test reports with Allure/Mochawesome
- Cross-browser testing
- Parallel execution support

---

## 👨‍💻 Author

- Siddharam Gurubhetti
- Contact: [siddhugurubhetti@gmail.com](mailto:siddhugurubhetti@gmail.com)
- GitHub: [siddhugurubhetti8483](https://github.com/siddhugurubhetti8483/saucedemo-cypress.git)
