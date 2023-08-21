### Class 41

#### Q1. Explain the concept of dynamic routes in Next.js and how they differ from static routes.

+ dynamic routes in Next.js provide a way to create pages with varying content based on parameters in the URL. They use square brackets [...] to define parameterized URLs, enabling flexible and personalized user experiences. Dynamic routes can be pre-rendered at build time (static generation) or at runtime (server-side rendering), allowing you to choose the optimal approach based on your data and performance needs. Static routes, in contrast, have fixed URLs and are pre-rendered at build time, making them efficient for delivering consistent content across pages.

---

#### Q2. Describe the process of deploying a Next.js application. What are the key steps involved, and what are some deployment platforms you can use?

The process of deploying a Next.js application:

Build: Generate production-ready files using the npm run build command.

Choose Platform: Select a deployment platform based on your application's needs.

Configure Environment: Set up environment variables, including API keys and credentials.

Deployment Method: Choose a deployment method based on static hosting, serverless deployment, or traditional hosting.

Deploy: Use platform-specific tools to upload your build files and assets to the hosting environment.

Domain and SSL: Configure a custom domain name and enable SSL for secure connections.

Monitor and Maintain: Keep an eye on performance, make necessary updates, and scale resources if required.

Deployment Platforms:

+ Vercel
+ Netlify
+ Heroku
+ GitHub Pages


---

#### Q3. How does Next.js handle static file serving? Discuss the default folder structure for storing static assets and explain how to reference them in a Next.js application.


Next.js handles static file serving by utilizing the public folder as the default location for storing static assets such as images, stylesheets, and fonts. These assets are accessible through the application's URL and are served directly by the server without being processed by build tools.

Key Points:

+ The public folder is located at the root level of the project directory.
+ Static assets placed in the public folder can be referenced directly in components.
+ The next/image component is used to optimize and load images efficiently.
+ HTML tags are used for referencing stylesheets, fonts, and other assets.
+ No need to include the /public prefix when referencing assets in the public folder.


