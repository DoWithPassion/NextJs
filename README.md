# NextJs
- Its a React framework for production.
- React is a library which essentially includes the components, states and props.
- And in react maximum features are from external packages. For routing, authentication and many other purposes.
- React gives interactivity for your frontend.

- Next Js is a *Full stack framework* for react js.
- *Framework* focuses on the huge things than the library. Which includes structure to you code and enhances the react features.
- Next JS solves the common problems of the *Reactjs* and makes building react apps easier.
- To make a react app for the *Production* ready, you need to solve may issues and organise/build the code accordingly. But the next js solves those issues for us.

## Features of NextJS.
- Next JS will provide some key features when compared to react.
### Built in serverside rendering
- Simply, Data fetching is done in the server and the finished up page will serve at the end.
- Allows to prerender the the react pages in the server side itself when it is loaded for the first time and then we can reduce the amount of time to get the data from the server(the time of loading state).
- Ofcourse, even in react there is a option or library to setup this. But needs some more configuration and setup to do this.
- So, Automatic page pre-rendering is done by the NextJS.
- NEXT JS improves the SEO for our websites.
### SEO
- Search Engine Optimization is the activity of optimizing your website to get more organic traffic from search engines. 
- SEO involves a lot of different techniques and aspects that we should pay attention to to make our website more attractive and accessible to a search engine.
- Single Page applications are pretty good but the search engines like google crawler processes will still have some lack of SEO results as it is a single initial page, the search engines cannot index the content because the single page applications will be rendered every time from the javascript when something changes.
- Ofcourse, single page applications had lot of advantages with the slower connections,save time, performance and better responsiveness but there will be some lack of good results in producing better seo results.

- In case of the nextjs the pages are statically generated or server rendered. So the page is initially loaded and it can be served easily to the users when they comeback from other pages easily.
- But we need to care some other features while using nextjs like meta tags, progressiveness, performance.
- The client side and server-side code are mixed up or blended with each other to render the finished pages.

### File Based Routing
- Instead of using the react router like in the react JS, In Next Js based on the files and folders in the pages folder of the project directory.
- Less Code and Highly understandable Routing feature.

### FullStack Capabilities
- We can easily add backend (server-side) code to your Next/React apps.
- Storing data, getting data, authentication etc can be added directly to the react apps instead of the seperate server code.
- We can use the Nodejs code in the next js project itself in the api directory of the pages.

## Installation
- First download the nodejs from the (Nodejs official website)[https://nodejs.org/en/].
- The next js requires the nodejs underhood to execute.
- Run the installer and once finished it, you are ready to start the next js.

## Creating a simple app
- To create a boiler plate nextjs project.
- Run `npx create-next-app`,
- Give a name to your project and after that your project will be constructed.

## IDE Setup
- You can use any modren ide of your choice. But I personally, not only me most of the developers prefer the Visual Studio Code.
- You can download it from the (official website)[https://code.visualstudio.com/download].
- Now open the project folder in the IDE.
- Modify the settings, view and preferences as you like.😊
- Install prettier extension in the extensions tab on the left side panel for better code formatting. And setup the shortcut for formatting in the settings>preferences> search formatting.

- Run `npm install` to make sure all the important modules that are mentioned as dependencies in the package.json are installed.

## Project Structure (Default from the create-next-app)
- Pages: The main folder that contains all our pages, file based routing and server code.
- Styles: Just some css stylesheets
- .gitignore - is a file used to ignore pushing some directories in to the github. Used when we are using git.
- Package.json - will contain the info of our project, dependencies and other scripts to run our project.
- Readme.md - Its just a file to write something about the project.
- Public - Contains some images and svgs. Unlike, React it doesnot contain the index.html file because the nextjs will have the builtin prerendering which gives the single page application that will be dynamically pre-rendered, when the first request from the server.

## Running next js
- Run the command `npm run dev` which will execute the `next dev` command which will gives us the great development experience as it watches for our changes and hot reload the app in the browser without rerunning the code again.
- When we are ready for going to production, we can run the `npm run build` which inturn execute `next build` command to build the optimised code output for deployment. 
- And to start the optimised deployment server, run `npm start` which in turn execute `next start`.
- You can make sure these npm commands and next commands mapping in the scripts section of the package.json

## React
- ReactJs is a client side javascript library which runs on the browser.
- It helps us to build modern reactive user interfaces for the website in an easier way.
- Its give a good structure to our code in a declarative and component focused approach.
- React controls entire frontend of a web application means each part of the webpage that we are looking can be done in react.
- It can follow widget approach (Some pages are rendered and served by the server and some are by the reactjs) or Single Page Applications Approach (Html page is sent by the server only once and thereafter, React takes over and controls the UI.)
- It is a components based UI library in which every thing is a component. And some other features are added via external packages available in the community.
- In react we write the  code in JSX(JavaScript XML) in which we mix up the react code with Javascript to make things easier.
- This JSX is converted to the HTML..behind the scenes while we are getting the view in browser.
- We can create a boiler plate code for the react project using `create-react-app` command.

### Boiler Plate code & Setup (Sample code setup)
- Make sure that nodejs is installed in your system
- Run the below command in the location where you wanted to create the project with boiler plate code.
    `npx create-react-app <Your Project Name Here>`
- After that go to the project folder and run the below command to start the development server (with the basic code got from the above command).
    `npm start`
- Now we can see the starting app in the browser and by default running in the port 3000.
- You can use the same settings with same IDE as we discussed for the NEXT JS in above section.

- NextJS is a framework, in that what we write is reactjs code.

