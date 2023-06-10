# Class 00

## Q1. What are the key characteristics of serverless computing, and how does it differ from traditional server-based architectures?

Serverless computing is a cloud computing model where the cloud provider manages the infrastructure and automatically allocates resources as needed. Key characteristics include:

+ No server management: Developers don't need to manage servers; the provider handles infrastructure tasks.
+ Event-driven execution: Functions are triggered by specific events, enabling efficient resource utilization.
+ Granular billing: Pay based on actual usage, resulting in cost savings.
+ Auto scaling: Infrastructure scales up or down automatically based on workload, improving performance and reducing costs.
+ Stateless execution: Functions don't maintain internal state, simplifying development and enabling easy scaling.
+ Microservices architecture: Applications are composed of small, independent functions or services.
+ Reduced operational overhead: Infrastructure management is abstracted, allowing developers to focus on application logic.
+ Rapid development and deployment: Allows for quick iteration and faster time-to-market.
+ Vendor lock-in: Migration between providers can be challenging due to differences in APIs and services.
Serverless computing offers convenience, scalability, and agility while abstracting away infrastructure management.


---

## Q2. How can one get started with Vercel, and what are the main steps involved in deploying a serverless function using Vercel?

+ Sign up for Vercel and install the CLI.
+ Set up your project with vercel init.
+ Write your serverless function in a dedicated file.
+ Test your function locally using vercel dev.
+ Deploy your function with vercel.
+ Monitor and manage deployments using the Vercel dashboard or CLI.
+ Vercel handles scaling and availability automatically.
+ Iterate and update your function by redeploying with vercel.

---

## Q3. What are APIs, and how can they be utilized in Python applications to access and manipulate data from external sources?

APIs (Application Programming Interfaces) are sets of rules that enable software applications to communicate with each other. In Python applications, you can utilize APIs to access and manipulate data from external sources through these steps:

+ Select the appropriate API for your data or functionality needs.
+ Read the API documentation to understand how to interact with it.
+ Install and import the necessary Python libraries for API communication.
+ Make API requests by sending HTTP requests to the API endpoints.
+ Handle the API responses, parse the data (often in JSON or XML format), and extract the relevant information.
+ Manipulate the retrieved data as required by your application.
+ Implement error handling to handle unexpected situations or errors.
+ Integrate the data into your application's logic or present it to the users.
By leveraging APIs in Python, you can access and manipulate external data, providing enhanced functionality and up-to-date information in your applications.
+ 

---

## Q4. What is the Requests library in Python, and how can it be used to interact with APIs by sending HTTP requests? Can you provide an example of a basic GET request using the Requests library?

The Requests library is a popular Python library for making HTTP requests. It simplifies the process of sending HTTP requests and handling responses, making it easier to interact with APIs. The library provides a high-level interface with various methods and options to send requests, handle parameters, headers, cookies, and more.

Example:

        import requests
        response = requests.get('URL')

        if response.status_code == 200:
            data = response()
            print(data)
        else:
            print('Error:', response.status_code)


