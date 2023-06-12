[Back to Home](../README.md)

# Web Scraping

1. Key differences between scraping static and dynamic websites:
   - Static websites: These websites are built using HTML and CSS, and the content remains the same unless manually updated. Scraping static websites involves downloading the HTML source code and extracting the desired information using techniques like regular expressions or HTML parsing libraries. The data extraction process is relatively straightforward since the content is fixed.
   - Dynamic websites: These websites use JavaScript to load and update content dynamically. The content is often retrieved from APIs or rendered on the client side. Scraping dynamic websites requires executing JavaScript code to fetch the dynamic content before extracting the desired information. Techniques like headless browsers or automated browser automation libraries like Playwright or Puppeteer are used to interact with the website and extract the data.

2. Techniques to avoid getting blocked while scraping websites:
   - Respect robots.txt: Check the website's `robots.txt` file to understand the scraping permissions. Adhering to the rules set in the `robots.txt` file helps maintain a good relationship with the website owner.
   - Limit request frequency: Avoid sending too many requests in a short period. Implement delays between requests to simulate human-like behavior and prevent overwhelming the server. Use techniques like randomized intervals or exponential backoff to vary the request timings.
   - Use proxy rotation: Utilize a pool of rotating IP addresses or proxy servers to distribute requests and avoid being detected as a single source. Proxies help hide your scraping activity and prevent IP-based blocking.

3. Playwright and its benefits in web scraping:
   Playwright is an open-source library for browser automation developed by Microsoft. It provides a high-level API for automating web browsers, including Chrome, Firefox, and WebKit. Playwright offers powerful features specifically designed for web scraping tasks:
   - Cross-browser compatibility: Playwright allows scraping websites using different browsers, giving flexibility in case a website behaves differently in different browsers.
   - Headless and headful modes: Playwright can run in headless mode, which doesn't display the browser UI, making it efficient for scraping. Alternatively, it can be used in headful mode, where the browser UI is visible, aiding in debugging and understanding website behavior.
   - Rich automation capabilities: Playwright provides methods for interacting with web elements, filling forms, navigating pages, and extracting data, making it suitable for complex scraping scenarios.

   Example use case: Scraping a website that relies heavily on JavaScript to load and display content. Playwright's ability to execute JavaScript and wait for dynamic content to load makes it beneficial in these cases. It can interact with the website, wait for asynchronous operations, and extract data from fully rendered pages.

4. Purpose of using XPath in web scraping and example expression:
   XPath is a query language for selecting nodes from an XML or HTML document. It allows you to navigate through the elements and attributes of an XML/HTML tree structure and extract specific data.

   Example XPath expression:
   Suppose you want to select all the links (`<a>` tags) within a specific `<div>` element with the class "content". The XPath expression would be:
   `//div[@class='content']//a`
   This expression selects all the `<a>` tags that are descendants of a `<div>` element with the class "content".