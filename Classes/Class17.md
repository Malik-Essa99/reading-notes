# Class 17

## Q1. What are the key differences between scraping static and dynamic websites?


+ Content: Static websites have fixed content, while dynamic websites generate content dynamically based on user interactions or external data.

+ Rendering: Static websites do not require client-side rendering, while dynamic we+ bsites rely on JavaScript to render content.

+ Data Retrieval: Scraping static websites involves parsing HTML source code, while scraping dynamic websites requires emulating or interacting with the dynamic behavior of the site using tools like headless browsers.

+ AJAX and APIs: Dynamic websites may use AJAX or APIs to fetch data, requiring additional steps to intercept and analyze these requests.

+ Maintenance: Static websites are generally easier to scrape and maintain, while dynamic websites require more effort due to frequent updates.

---

## Q2. Explain at least three techniques or best practices that can be employed to avoid getting blocked while scraping websites.

+ Respect Robots.txt: Adhere to the directives specified in a website's Robots.txt file, which outlines areas that are off-limits for crawling.

+ Implement Rate Limiting: Slow down the rate of your scraping requests by adding delays between each request or setting a maximum number of requests per minute to avoid triggering rate-limiting mechanisms.

+ Use User-Agent Rotation: Rotate the User-Agent header with each request to make it appear as if different browsers or devices are accessing the website, helping to mask your scraping activity.

---

## Q3. What is Playwright, and how does it assist in web scraping tasks? Provide an example of a use case where Playwright would be particularly beneficial.

Playwright is an automation framework that allows you to control web browsers programmatically. It is particularly beneficial for web scraping tasks that involve dynamic websites relying on JavaScript for content rendering. Playwright's API enables you to interact with web pages, trigger dynamic content loading, and extract information from the rendered elements. It overcomes the limitations of traditional scraping libraries when dealing with JavaScript-heavy websites, making it a valuable tool for web scraping tasks.

Example:

Imagine you want to scrape data from a real estate website that dynamically loads property listings as users scroll down the page. Traditional scraping methods may only capture the initially loaded properties and miss the dynamically loaded ones.

Using Playwright, you can automate the scrolling and data extraction process. Here's how it would work:

+ Launch a browser instance using Playwright's API.
+ Navigate to the real estate website and wait for the property listings to load.
+ Use Playwright's API to simulate scrolling down the page to trigger the loading of additional property listings.
+ Wait for the dynamically loaded listings to appear.
+ Extract the desired data from the property listings, such as property details, prices, and locations, using Playwright's API.
+ Repeat the scrolling and extraction process until all desired listings are captured.

---

## Q4. Describe the purpose of using Xpath in web scraping, and provide an example of an Xpath expression to select a specific HTML element from a webpage.

Xpath is a query language used in web scraping to locate and extract specific elements or data from HTML documents. It allows you to navigate the structure of the document and target elements based on their attributes or relationships. An example Xpath expression to select a specific HTML element, such as a title, would be: //div[@class="blog-post"]/h2. This expression selects the h2 element with the title of the blog post from the given HTML snippet. Xpath provides a powerful and precise way to retrieve desired information from web pages during scraping.

Example: 

        <div class="product">
            <h2>Product Title</h2>
            <p class="price">$49.99</p>
        </div>

To select the title element

        //div[@class="product"]/p[@class="price"]

