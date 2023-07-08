# Class 26

### Q1. What are the key components of the Django framework, and how do they contribute to building a web application?


+ Models: Define the data structure and handle database operations.
+ Views: Handle request processing, interact with models, and generate responses.
+ Templates: Generate dynamic HTML pages by integrating data and logic.
+ URL Dispatcher: Map URLs to appropriate views.
+ Forms: Handle user input, validation, and rendering of form elements.
+ Middleware: Modify requests and responses between the web server and Django's view processing.
+ Authentication and Authorization: Provide user authentication and permission management.
+ Admin Interface: Ready-to-use administrative interface for managing site content.

---

### Q2. Explain the role of Django’s MTV (Model-View-Template) architecture and how it handles a typical web request-response cycle.

Django's MTV architecture separates concerns into models, views, and templates, enabling code organization, reusability, and maintainability throughout web development.

+ Model: Represents the data and interacts with the database.
+ Template: Manages the presentation logic and generates the user interface.
+ View: Contains the application logic and orchestrates models and templates.

Request response cycle:

1. User sends a request to a specific URL.
2. Django's URL dispatcher maps the URL to the appropriate view.
3. The view function or class receives the request and processes data.
4. It interacts with models to retrieve or update data if needed.
5. The view selects the template for rendering the response.
6. The template generates HTML by incorporating dynamic data.
7. The rendered HTML is sent back as a response to the user's browser.
8. The browser receives the response and displays the rendered HTML page.

---

### Q3. What is the purpose of Tailwind CSS, and how does it differ from Bootstrap CSS?

+ Tailwind CSS focuses on providing a utility-first approach, offering a wide range of customizable utility classes for building unique UIs.
+ Bootstrap CSS offers pre-designed components and a default theme, aiming to streamline front-end development with ready-to-use components and a consistent design system.



