+++
title = 'Cors'
date = 2023-12-24T22:21:43+05:30
draft = true
+++
## Same-Origin Policy (SOP)

- **Definition:**
  - Fundamental security policy in web browsers.
  - Restricts web pages from making requests to different origins (domains, protocols, ports) than the one that served the web page.
  
- **Purpose:**
  - Prevents malicious scripts from accessing or manipulating data across different origins.
  
- **Impact:**
  - Blocks cross-origin requests by default to ensure security.
  
- **Workarounds:**
  - CORS (Cross-Origin Resource Sharing) headers on the server-side explicitly allow certain origins to access resources.
  - Proxy servers can be used to make requests appear to come from the same origin.

---

## Cross-Origin Requests and Handling Errors

- **Error: Undefined Request Body (POST and PUT Requests):**
  - Occurs when server-side code fails to handle or parse data sent in the request body.
  
- **Solutions:**
  - **CORS Headers:**
    - Configure server-side API to include appropriate CORS headers.
  - **Proxy Servers:**
    - Use a server-side proxy to make requests appear to come from the same origin.
  - **Data Handling:**
    - Ensure proper parsing and handling of request body data.
    - Libraries like `body-parser` in Node.js help parse incoming request bodies.
    
- **Preventing Errors and SOP Issues:**
  - Addressing SOP restrictions:
    - Implement CORS headers on the server-side.
    - Use appropriate access controls to permit specific origins.
  - Properly handling request data:
    - Validate and parse incoming request bodies to prevent "undefined" errors.
    - Handle errors gracefully to provide meaningful feedback to users.
