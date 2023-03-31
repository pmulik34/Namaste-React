## Namaste React Course by Akshay Saini
# _Chapter 01 - Inception_

## Q: What is `Emmet`?
ans: Emmet is tool that helps developers write HTML and CSS code more quickly and easily. It works by letting developers use short abbreviations instead of typing out long lines of code. Then with the click of button or the press of a key, Emmet can expand these abbreviations into full HTML and CSS code. This can save a lot of time and make coding less tedious.


## Q: What is `CDN`? Why do we use it?
ans: A `CDN (Content Delivery Network)` is a network of servers distributed across various geographical locations that work together to deliver content (such as images, videos, or other files) to users more efficiently and quickly.

Here's an example of how a CDN works:

When you visit a website that uses a CDN to deliver its content, your request for a file (such as an image) is automatically routed to the nearest server within the CDN. This server then retrieves the file from the website's origin server and delivers it to your browser. Since the server is closer to you, the file is delivered more quickly and efficiently than if it had to travel a longer distance from the website's origin server.

CDNs are used for a number of reasons, including:

    1.Improved website performance: By delivering content from servers that are closer to users, CDNs can improve website load times and reduce latency, which can lead to a better user experience.

    2.Reduced server load: CDNs can help reduce the load on a website's origin server by distributing content across multiple servers. This can help prevent server overload and improve website uptime.

    3.Increased scalability: CDNs can help websites handle large amounts of traffic more easily by distributing content across multiple servers.

Overall, CDNs help make the internet faster and more reliable for users by delivering content more efficiently and reducing website downtime.


## Q: What is `crossorigin in script tag`?
ans : When you include a JavaScript file on a webpage using a `<script>` tag, the browser downloads and executes that file. If the file is hosted on the same domain as the webpage, the browser assumes that it can be trusted and runs it without any issues.

However, if the file is hosted on a different domain than the webpage, the browser needs to determine whether it can trust that file. This is where the crossorigin attribute comes in.

By setting the `crossorigin` attribute to either `anonymous` or `use-credentials`, you are telling the browser whether or not the JavaScript file can be trusted to access sensitive data (such as cookies) on the user's browser.

If you set `crossorigin="anonymous"`, the browser will download and execute the script, but will not allow it to access any sensitive data on the user's browser. This is useful if you are loading a script from a third-party domain that you don't completely trust.

If you set `crossorigin="use-credentials"`, the browser will download and execute the script, and will allow it to access sensitive data on the user's browser. This is useful if you are loading a script from a trusted domain that needs to access sensitive data on the user's browser.

When `crossorigin` is specified without a value, it defaults to `anonymous`.

## Why React created two different CDN files ?
React was initially designed for use in web applications, and it was packaged as a single library that included everything needed for rendering components in a web browser.

However, when React was introduced for mobile development, a separate library called React Native was created. This is because mobile apps have different requirements than web apps, and React Native was designed specifically for mobile development.

To support the creation of React Native, React was split into two separate libraries: React and ReactDOM. React contains the core functionality of React and can be used in both web and mobile applications. ReactDOM is a library specifically designed for rendering React components in web applications.

By separating React and ReactDOM, developers can write components that can be shared between the web version of React and React Native, allowing for more efficient code reuse and easier maintenance.
