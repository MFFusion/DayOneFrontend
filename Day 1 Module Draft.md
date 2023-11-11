
### 1. Learning Outcomes

#### 1.1 Understanding Reactivity in a Web App
   - **Explanation:**
     - Define reactivity in the context of a web application.
     - Discuss the concept of data-binding and how it enables automatic UI updates.
     - Explore the reactivity system in VueJS, including the reactivity caveats.

   - **Activities:**
     - Create a simple Vue component to demonstrate reactivity.
     - Modify data properties and observe how the UI updates reactively.

#### 1.2 Ability to develop a frontend application using HTML, CSS, JavaScript
   - **Explanation:**
     - Emphasize the role of VueJS as a progressive framework, allowing integration into existing projects.
     - Discuss the HTML template syntax, styling with CSS, and enhancing functionality with JavaScript within Vue components.

   - **Activities:**
     - Build a basic VueJS application incorporating HTML, CSS, and JavaScript.
     - Customize the styling of components using scoped CSS.

#### 1.3 Understanding how routing works, and how to use it
   - **Explanation:**
     - Introduce Vue Router and its significance in single-page applications.
     - Explain the concept of routing, navigation guards, and nested routes.

   - **Activities:**
     - Set up Vue Router in a project.
     - Create multiple pages and link them using router links.
     - Implement navigation guards for authentication or data validation.

#### 1.4 Making API Requests with Fetch API (replacing state management)
   - **Explanation:**
     - Introduce the Fetch API for making asynchronous HTTP requests.
     - Discuss the basics of making GET, POST, and other types of requests.
     - Explain how to handle responses and errors.

   - **Activities:**
     - Integrate the Fetch API into a VueJS application to retrieve data from a mock API.
     - Implement data binding to display the fetched data in the UI.

### General Tips for Day 1 Facilitation:

- **Hands-On Exercises:** Continue to incorporate hands-on exercises for each learning outcome, focusing on using the Fetch API.

- **Real-world Examples:** Utilize real-world examples to illustrate the practical applications of VueJS and API integration.

- **Peer Collaboration:** Encourage participants to collaborate and discuss their solutions during the activities.

- **Q&A Sessions:** Allocate time for questions and answers to address any confusion or concerns related to API integration.

- **Resources for Further Learning:** Provide additional resources and references for participants interested in diving deeper into VueJS and API interactions.

- **Feedback Loop:** Maintain a feedback loop for participants to share their thoughts on the learning materials and session structure.

# Beginning VueJS

## Some short notes

VueJS is a JavaScript \*framework for building Single Page Application for the web. It uses HTML, CSS, JSS and uses both component-based and declarative programming model to build user interfaces. It is a progressive framework, which means that it is both flexible and *incrementally* adoptable. These are the uses for VueJS
- Enhancing static HTML without a build step
- Embedding as Web Components on any page
- Single-Page Application (SPA)
- Fullstack / Server-Side Rendering (SSR)
- Jamstack / Static Site Generation (SSG)
- Targeting desktop, mobile, WebGL, and even the terminal
\*A framework is just a structured way of writing JavaScript code. Different frameworks does the same things (which is building interactive web application) differently, with different goals in mind.

## Before we begin

1) Install NPM, as this will be the only way we will install JS library, frameworks, and packages throughout this workshop

## Setting up a VueJS project

For this workshop, we will be using Vite.

### What is Vite?

I copied this from Wikipedia :
**Vite** (French: [[vit]](https://en.wikipedia.org/wiki/Help:IPA/French "Help:IPA/French"), like "veet") is a local development server written by Evan You, the creator of [Vue.js](https://en.wikipedia.org/wiki/Vue.js "Vue.js"), and used by default by [Vue](https://en.wikipedia.org/wiki/Vue.js "Vue.js") and for [React](https://en.wikipedia.org/wiki/React_(software) "React (software)") project templates. It has support for [TypeScript](https://en.wikipedia.org/wiki/TypeScript "TypeScript") and [JSX](https://en.wikipedia.org/wiki/JSX_(JavaScript) "JSX (JavaScript)"). It uses Rollup and [esbuild](https://en.wikipedia.org/wiki/Esbuild "Esbuild") internally for bundling.

It monitors files as they're being edited and upon file save the web browser reloads the code being edited through a process called Hot Module Replacement (HMR) which works by just reloading the specific file being changed using ES6 modules (ESM) instead of recompiling the entire application.

Vite provides built-in support for server-side rendering (SSR). By default, it listens on TCP port 5173. It is possible to configure Vite to serve content over [HTTPS](https://en.wikipedia.org/wiki/HTTPS "HTTPS") and proxy requests (including [WebSocket](https://en.wikipedia.org/wiki/WebSocket "WebSocket")) to a back-end web server (such as [Apache HTTP Server](https://en.wikipedia.org/wiki/Apache_HTTP_Server "Apache HTTP Server") or [lighttpd](https://en.wikipedia.org/wiki/Lighttpd "Lighttpd")).

### Vite for VueJS

Open *PowerShell* and run the command _npm create vite@latest_ and press ENTER. This should prompt you to setup a name for your project, and select VueJS when the prompt is shown. Afterwards, you may choose TypeScript, or JavaScript (depending on how much you like to suffer). Vite will then create a new folder containg your VueJS project scaffold. Before you start, make sure to run *cd* into the project folder Vite just made and run the command *npm i* to install any missing dependencies for your project.

After setting up your VueJS project, you should find

