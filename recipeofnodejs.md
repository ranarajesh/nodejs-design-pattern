The Node.js recipe
The fundamental building blocks of Node.js are the reactor design and libuv, however three additional elements are required to construct the entire platform:

• A collection of bindings that give JavaScript access to libuv and other low-level features.

• V8, the JavaScript engine that Google first created for the Chrome web browser. This contributes to Node.js's speed and effectiveness. V8 is praised for its quickness, innovative design, and effective memory management.

The Node.js API at a high level is implemented by a core JavaScript library.

This is the recipe for making Node.js, and the finished architecture is shown in the accompanying figure: