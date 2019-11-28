# Zero dependency front-end components with Web Components

*sthlm.js Nov 27, 2019*

## Web standards and vanilla JS FTW!

> HTML, JS, CSS, Layout (Blisk), JS (V8), APIs (including of course web components) all for free in the browser.

You're given a web browser with a JS engine, a rendering engine, and APIs. APIs for DOM manipulation, network IO, storage and caching, and much much more. All of it based on open standards that are thought-out and universally agreed upon. One of the things that can be done natively in vanilla JS with web platform APIs is to create encapsulated frontend components. This collection of standards is called Web Components.

**So let's see what the browser can actually do!**

## Web components are nothing complicated, just a few building blocks

> Custom Elements API, Shadow DOM and template tags. That’s it. Use vanilla JS for the rest.

As you might have guessed, one alternative to frontend frameworks is to use web components. Just as any framework, web components allow us to create encapsulated and reusable components.

Web components is the term for the building blocks built into the web platform that enable us to create browser-native frontend components. The building blocks are: 

- The Custom Elements API, used for creating and registering the components
- The Shadow DOM, used for encapsulating style and document structure
- And the template tag, for re-using HTML elements efficiently

Use vanilla JS and web platform APIs (such as the DOM API) for all the rest. This is all built right into the browser.

**This doesn’t solve anything new, right? Well, I think it’s pretty big to have all of this built into the browser. No magic, no build tools, just vanilla HTML/JS/CSS. And also…**

## Web components are freaking fun!

> Also, they enable you to design code the way the web platform was designed to be used.

For me, this is super interesting because I think it’s fun! Not only does it fit well with my love for simplicity and hate for “magic”, I absolutely love to do things at the lowest feasible layer of abstraction. Meaning, using things the platform provides when possible.

But in a more serious sense, I think it’s our duty as frontend developers to know how the browser works and what we can do with it. And experimenting with web components also forces (although I like to use the term “enables”) us to use the web standards the way they were designed to be used. Passing data mainly as element attributes, reacting to events via event listeners, and so on. And remember, this also means no dependencies and no build tools.

**See [sample code](https://github.com/ericselin/web-components-sthlmjs/blob/master/index.html) and [more examples](https://github.com/ericselin/web-components-sthlmjs/tree/master/examples) in the [GitHub repo](https://github.com/ericselin/web-components-sthlmjs)!**

## Web components have been around for a long time and are picking up speed

> Accelerated Mobile Pages, Polymer, Stencil and e.g. Salesforce Lightning Web Components are all based on web components.

Web components have been around for a long time and it’s now a mature way to create components. It’s included in the HTML Living Standard and other applicable specifications. Browser support is great – all the major browsers support it. And you can polyfill most of the spec even for IE. After a slow start it’s picking up speed.

AMP, Polymer and Stencil all use web components. Svelte can compile to a web component target. And because it’s such a low overhead way to create components, it’s a great fit for design systems – e.g. Salesforce uses web components for their design elements.

> So for your next prototype or personal project, write vanilla HTML/JS/CSS, use native APIs and have fun experimenting!

---

## Appendix

### Resources

[google.com/search?q=web+components](https://google.com/search?q=web+components)

[developer.mozilla.org/en-US/docs/Web/Web_Components](https://developer.mozilla.org/en-US/docs/Web/Web_Components)

[developers.google.com/web/fundamentals/web-components/](https://developers.google.com/web/fundamentals/web-components/)

[webcomponents.org](https://www.webcomponents.org)

[ericselin.dev](https://ericselin.dev)

### Side note on frameworks

Frameworks and libraries are great, but make things more complicated.

> External dependencies create bigger codebases and islands of “magic”.

We have a great ecosystem around JS these days. You don’t need to reinvent the wheel and can “stand on the shoulder of giants” to achieve what you need. However, just “npm installing” everything is seldom the answer. It can make your code more complicated rather than more simple if you’re not careful.

1. For one, it creates these islands of “magic”. With how things actually work, with building your app for production, and with development itself.
2. Also, the code you ship inevitably grows in size and complexity. Not very good in todays mobile-first world.
3. Finally, no tool is a one-size-fits-all. In the best case, you create clunky workarounds, and in the worst case, you have to compromise on your vision.

**Frameworks and libraries are great, but there are simpler solutions that may suit your use-case even better.**