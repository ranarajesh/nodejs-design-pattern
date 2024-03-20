Module systems in JavaScript and Node.js#
JavaScript Module Evolution:
Historically, JavaScript lacked a built-in module system, relying on <script> tags for file inclusion in browsers.
As web applications grew in complexity, initiatives like AMD (Asynchronous module definition)and UMD(Universal Module Definition) emerged to define module systems for JavaScript projects.
These initiatives aimed to address the increasing complexity of JavaScript applications, especially with the rise of frameworks like jQuery, Backbone, and AngularJS.
Node.js Module System:
Node.js introduced a unique module system, diverging from browser-based approaches, relying on JavaScript files available in the local filesystem.
Node.js adopted the CommonJS specification for its module system, providing a standardized approach for managing modules in browserless environments.
CommonJS gained prominence not only in Node.js but also in the browser landscape, facilitated by module bundlers like Browserify and webpack.
ESM (ECMAScript Modules):
With the release of ECMAScript 6 (ES2015), ESM emerged as the official proposal for a standard module system.
ESM aims to bridge the gap between browser and server module management.
While ECMAScript 6 defined the specification for ESM syntax and semantics, it lacked implementation details.
It took several years for browsers and the Node.js community to implement ESM support, with Node.js introducing stable ESM support from version 13.2 onwards.
Modules for Structuring Applications:
Modules are essential for organizing non-trivial applications and enforcing information hiding by keeping private functions and variables inaccessible unless explicitly exported.
The Revealing Module Pattern:
Addresses the lack of namespacing in JavaScript, where every script runs in the global scope, risking pollution and unpredictable behavior.
Utilizes a self-invoking function (IIFE) to create a private scope, exporting only designated parts publicly.
Variables created inside the function are not accessible from outside, ensuring privacy.
Functions use the return statement to selectively expose information to the outer scope, exporting only the public API.
Example:
