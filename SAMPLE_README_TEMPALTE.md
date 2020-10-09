Flutter Guide
==

[![Front End Developer Desk](https://raw.githubusercontent.com/flutter/website/master/src/_assets/image/flutter-lockup.png)](https://dribbble.com/shots/3577639-Isometric-Developer-Desk)

_Credits: [Illustration](https://dribbble.com/shots/3577639-Isometric-Developer-Desk) by [@yangheng](https://dribbble.com/yangheng)_

_This guide has been cross-posted on [Free Code Camp](https://medium.freecodecamp.com/grabs-front-end-guide-for-large-teams-484d4033cc41)._

[Grab](https://www.grab.com) is Southeast Asia (SEA)'s leading transportation platform and our mission is to drive SEA forward, leveraging on the latest technology and the talented people we have in the company. As of May 2017, we handle [2.3 million rides daily](https://www.bloomberg.com/news/videos/2017-05-11/tans-says-company-has-more-than-850-000-drivers-video) and we are growing and hiring at a rapid scale.


This study guide is inspired by ["A Study Plan to Cure JavaScript Fatigue"](https://medium.freecodecamp.com/a-study-plan-to-cure-javascript-fatigue-8ad3a54f2eb1#.g9egaapps) and is mildly opinionated in the sense that we recommend certain libraries/frameworks to learn for each aspect of front end development, based on what is currently deemed most suitable at Grab. We explain why a certain library/framework/tool is chosen and provide links to learning resources to enable the reader to pick it up on their own. Alternative choices that may be better for other use cases are provided as well for reference and further self-exploration.

If you are familiar with front end development and have been consistently keeping up with the latest developments, this guide will probably not be that useful to you. It is targeted at newcomers to front end.



*- Grab Web Team*

**Pre-requisites**

- Good understanding of core programming concepts.
- Comfortable with basic command line actions and familiarity with source code version control systems such as Git.
- Experience in web development. Have built server-side rendered web apps using frameworks like Ruby on Rails, Django, Express, etc.
- Understanding of how the web works. Familiarity with web protocols and conventions like HTTP and RESTful APIs.

### Table of Contents

- [About Flutter](#about-flutter)
- [Study Plan Overview](#study-plan-overview)
- [Flutter Roadmap](#flutter-roadmap)
- [Youtube Channels to Subscribe](#youtube-channels-to-subscribe)
- [Good Bloggers to Follow ](#good-bloggers-to-follow)
- [Other important websites](#other-important-websites)
- [The Journey has Just Begun](#the-journey-has-just-begun)

Certain topics can be skipped if you have prior experience in them.

## About Flutter

Web developers these days refer to the products they build as web apps, rather than websites. While there is no strict difference between the two terms, web apps tend to be highly interactive and dynamic, allowing the user to perform actions and receive a response for their action. Traditionally, the browser receives HTML from the server and renders it. When the user navigates to another URL, a full-page refresh is required and the server sends fresh new HTML for the new page. This is called server-side rendering.

However in modern SPAs, client-side rendering is used instead. The browser loads the initial page from the server, along with the scripts (frameworks, libraries, app code) and stylesheets required for the whole app. When the user navigates to other pages, a page refresh is not triggered. The URL of the page is updated via the [HTML5 History API](https://developer.mozilla.org/en-US/docs/Web/API/History_API). New data required for the new page, usually in JSON format, is retrieved by the browser via [AJAX](https://developer.mozilla.org/en-US/docs/AJAX/Getting_Started) requests to the server. The SPA then dynamically updates the page with the data via JavaScript, which it has already downloaded in the initial page load. This model is similar to how native mobile apps work.

The benefits:

- The app feels more responsive and users do not see the flash between page navigations due to full-page refreshes.
- Fewer HTTP requests are made to the server, as the same assets do not have to be downloaded again for each page load.
- Clear separation of the concerns between the client and the server; you can easily build new clients for different platforms (e.g. mobile, chatbots, smart watches) without having to modify the server code. You can also modify the technology stack on the client and server independently, as long as the API contract is not broken.

The downsides:

- Heavier initial page load due to loading of framework, app code, and assets required for multiple pages.<sup><a href="#fn1" id="ref1">1</a></sup>
- There's an additional step to be done on your server which is to configure it to route all requests to a single entry point and allow client-side routing to take over from there.
- SPAs are reliant on JavaScript to render content, but not all search engines execute JavaScript during crawling, and they may see empty content on your page. This inadvertently hurts the Search Engine Optimization (SEO) of your app. <sup><a href="#fn2" id="ref2">2</a></sup>. However, most of the time, when you are building apps, SEO is not the most important factor, as not all the content needs to be indexable by search engines. To overcome this, you can either server-side render your app or use services such as [Prerender](https://prerender.io/) to "render your javascript in a browser, save the static HTML, and return that to the crawlers".

While traditional server-side rendered apps are still a viable option, a clear client-server separation scales better for larger engineering teams, as the client and server code can be developed and released independently. This is especially so at Grab when we have multiple client apps hitting the same API server.

As web developers are now building apps rather than pages, organization of client-side JavaScript has become increasingly important. In server-side rendered pages, it is common to use snippets of jQuery to add user interactivity to each page. However, when building large apps, just jQuery is insufficient. After all, jQuery is primarily a library for DOM manipulation and it's not a framework; it does not define a clear structure and organization for your app.

JavaScript frameworks have been created to provide higher-level abstractions over the DOM, allowing you to keep state in memory, out of the DOM. Using frameworks also brings the benefits of reusing recommended concepts and best practices for building apps. A new engineer on the team who is unfamiliar with the code base, but has experience with a framework, will find it easier to understand the code because it is organized in a structure that they are familiar with. Popular frameworks have a lot of tutorials and guides, and tapping on the knowledge and experience from colleagues and the community will help new engineers get up to speed.

#### Usefull Blogs about flutter

- [Single Page App: advantages and disadvantages](http://stackoverflow.com/questions/21862054/single-page-app-advantages-and-disadvantages)
- [The (R)Evolution of Web Development](http://blog.isquaredsoftware.com/presentations/2016-10-revolution-of-web-dev/)
- [Here's Why Client Side Rendering Won](https://medium.freecodecamp.com/heres-why-client-side-rendering-won-46a349fadb52)

## Study Plan Overview

Explain the study plan and how to go about the entire things , attach dynamic links to the other sections of the doc as well for eg- a dynamic link to the roadmap .

#### Courses Links
    Do these courses in the following order 

- [Learn ES5 on Codecademy](https://www.codecademy.com/learn/learn-javascript)
- [Learn ES6 on Codecademy](https://www.codecademy.com/learn/introduction-to-javascript)
- [Learn ES2015 on Babel](https://babeljs.io/learn-es2015/)
- [ES6 Katas](http://es6katas.org/)
- [You Don't Know JS](https://github.com/getify/You-Dont-Know-JS) (Advanced content, optional for beginners)
- [Answers to Front End Job Interview Questions — JavaScript](https://github.com/yangshun/front-end-interview-handbook/blob/master/questions/javascript-questions.md)

#### Sample Project Links

    Do these projects to attain a greater grasp over the concepts

- [Learn ES5 on Codecademy](https://www.codecademy.com/learn/learn-javascript)
- [Learn ES6 on Codecademy](https://www.codecademy.com/learn/introduction-to-javascript)
- [Learn ES2015 on Babel](https://babeljs.io/learn-es2015/)
- [ES6 Katas](http://es6katas.org/)
- [You Don't Know JS](https://github.com/getify/You-Dont-Know-JS) (Advanced content, optional for beginners)
- [Answers to Front End Job Interview Questions — JavaScript](https://github.com/yangshun/front-end-interview-handbook/blob/master/questions/javascript-questions.md)

## Flutter Roadmap 

<img alt="React Logo" src="https://raw.githubusercontent.com/Tarikul711/flutter-development-roadmap/master/docs/flutter-app-development-roadmap-by-tarikul.png"  />

Expain the roadmap

If any JavaScript project has taken the front end ecosystem by storm in recent years, that would be [React](https://facebook.github.io/react/). React is a library built and open-sourced by the smart people at Facebook. In React, developers write components for their web interface and compose them together.

React brings about many radical ideas and encourages developers to [rethink best practices](https://www.youtube.com/watch?v=DgVS-zXgMTk). For many years, web developers were taught that it was a good practice to write HTML, JavaScript and CSS separately. React does the exact opposite, and encourages that you write your HTML and [CSS in your JavaScript](https://speakerdeck.com/vjeux/react-css-in-js) instead. This sounds like a crazy idea at first, but after trying it out, it actually isn't as weird as it sounds initially. Reason being the front end development scene is shifting towards a paradigm of component-based development. The features of React:

- **Declarative** - You describe what you want to see in your view and not how to achieve it. In the jQuery days, developers would have to come up with a series of steps to manipulate the DOM to get from one app state to the next. In React, you simply change the state within the component and the view will update itself according to the state. It is also easy to determine how the component will look like just by looking at the markup in the `render()` method.

- **Functional** - The view is a pure function of `props` and `state`. In most cases, a React component is defined by `props` (external parameters) and `state` (internal data). For the same `props` and `state`, the same view is produced. Pure functions are easy to test, and the same goes for functional components. Testing in React is made easy because a component's interfaces are well-defined and you can test the component by supplying different `props` and `state` to it and comparing the rendered output.

- **Maintainable** - Writing your view in a component-based fashion encourages reusability. We find that defining a component's `propTypes` make React code self-documenting as the reader can know clearly what is needed to use that component. Lastly, your view and logic is self-contained within the component, and should not be affected nor affect other components. That makes it easy to shift components around during large-scale refactoring, as long as the same `props` are supplied to the component.

React is a library, not a framework, and does not deal with the layers below the view - the app state. More on that later.

**Estimated Duration: 3-4 days.** Try building simple projects like a to-do list, Hacker News clone with pure React. You will slowly gain an appreciation for it and perhaps face some problems along the way that isn't solved by React, which brings us to the next topic...

#### Study Links

- [React Official Tutorial](https://facebook.github.io/react/tutorial/tutorial.html)
- [Egghead Course - Build Your First Production Quality React App](https://egghead.io/courses/build-your-first-production-quality-react-app)
- [Simple React Development in 2017](https://hackernoon.com/simple-react-development-in-2017-113bd563691f)
- [Presentational and Container Components](https://medium.com/@dan_abramov/smart-and-dumb-components-7ca2f9a7c7d0#.5iexphyg5)

#### Alternatives

- [Angular](https://angular.io/)
- [Ember](https://www.emberjs.com/)
- [Vue](https://vuejs.org/)
- [Cycle](https://cycle.js.org/)

## Youtube Channels to Subscribe

<img alt="Redux Logo" src="https://i.insider.com/59a59a8d79bbfd1d008b601a?width=1200&format=jpeg" width="256px" />

Importance of Youtube Channels mock contect same in eaxh readme.

- **[Channel Name 1](https://developer.mozilla.org/en-US/docs/Web/API/History_API)** - Brief Description about the channel.
- **[Channel Name 2](https://developer.mozilla.org/en-US/docs/Web/API/History_API)** - Brief description about the channel.
- **[Channel Name 2](https://developer.mozilla.org/en-US/docs/Web/API/History_API)** - Brief description about the channel.


## Good Bloggers to Follow 

<img alt="Redux Logo" src="https://miro.medium.com/max/968/1*uLuWzCXfq2rt1t_TkuLB8A.png" width="256px" />

Importance of Youtube Channels mock contect same in eaxh readme.

- **[Blogger Name 1](https://developer.mozilla.org/en-US/docs/Web/API/History_API)** - Brief Description about the Blogger.
- **[Blogger Name 2](https://developer.mozilla.org/en-US/docs/Web/API/History_API)** - Brief description about the channel.
- **[Channel Name 2](https://developer.mozilla.org/en-US/docs/Web/API/History_API)** - Brief description about the channel.


## Other important websites 

<img alt="Redux Logo" src="https://miro.medium.com/max/1200/0*UEtwA2ask7vQYW06.png" width="256px" />

Importance of Youtube Channels mock contect same in eaxh readme.

- **[Blogger Name 1](https://developer.mozilla.org/en-US/docs/Web/API/History_API)** - Brief Description about the Blogger.
- **[Blogger Name 2](https://developer.mozilla.org/en-US/docs/Web/API/History_API)** - Brief description about the channel.
- **[Channel Name 2](https://developer.mozilla.org/en-US/docs/Web/API/History_API)** - Brief description about the channel.


### The Journey has Just Begun

Congratulations on making it this far! Front end development today is [hard](https://hackernoon.com/how-it-feels-to-learn-javascript-in-2016-d3a717dd577f), but it is also more interesting than before. What we have covered so far will help any new engineer to Grab's web team to get up to speed with our technologies pretty quickly. There are many more things to be learnt, but building up a solid foundation in the essentials will aid in learning the rest of the technologies. This helpful [front end web developer roadmap](https://github.com/kamranahmedse/developer-roadmap#-front-end-roadmap) shows the alternative technologies available for each aspect.

We made our technical decisions based on what was important to a rapidly growing Grab Engineering team - maintainability and stability of the code base. These decisions may or may not apply to smaller teams and projects. Do evaluate what works best for you and your company.

As the front end ecosystem grows, we are actively exploring, experimenting and evaluating how new technologies can make us a more efficient team and improve our productivity. We hope that this post has given you insights into the front end technologies we use at Grab. If what we are doing interests you, [we are hiring](https://grab.careers)!

*Many thanks to [Joel Low](https://github.com/lowjoel), [Li Kai](https://github.com/li-kai) and [Tan Wei Seng](https://github.com/xming13) who reviewed drafts of this article.*

### More Reading

**General**

- [State of the JavaScript Landscape: A Map for Newcomers](http://www.infoq.com/articles/state-of-javascript-2016)
- [The Hitchhiker's guide to the modern front end development workflow](http://marcobotto.com/the-hitchhikers-guide-to-the-modern-front-end-development-workflow/)
- [How it feels to learn JavaScript in 2016](https://hackernoon.com/how-it-feels-to-learn-javascript-in-2016-d3a717dd577f#.tmy8gzgvp)
- [Roadmap to becoming a web developer in 2017](https://github.com/kamranahmedse/developer-roadmap#-frontend-roadmap)
- [Modern JavaScript for Ancient Web Developers](https://trackchanges.postlight.com/modern-javascript-for-ancient-web-developers-58e7cae050f9)

**Other Study Plans**

- [A Study Plan To Cure JavaScript Fatigue](https://medium.freecodecamp.com/a-study-plan-to-cure-javascript-fatigue-8ad3a54f2eb1#.c0wnrrcwd)
- [JS Stack from Scratch](https://github.com/verekia/js-stack-from-scratch)
- [A Beginner’s JavaScript Study Plan](https://medium.freecodecamp.com/a-beginners-javascript-study-plan-27f1d698ea5e#.bgf49xno2)

### Footnotes

<p id="fn1">1. This can be solved via <a href="https://webpack.js.org/guides/code-splitting/">webpack code splitting</a>. <a href="#ref1" title="Jump back to footnote 1 in the text.">↩</a></p>

<p id="fn2">2. <a href="https://medium.com/@mjackson/universal-javascript-4761051b7ae9">Universal JS</a> to the rescue! <a href="#ref2" title="Jump back to footnote 1 in the text.">↩</a></p>