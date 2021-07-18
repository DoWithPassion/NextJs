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

### Context
- React Context is a method to pass props from parent to child component(s), by storing the props in a store(similar in Redux) and using these props from the store by child component(s) without actually passing them manually at each level of the component tree.

### Boiler Plate code & Setup (Sample code setup)
- Make sure that nodejs is installed in your system
- Run the below command in the location where you wanted to create the project with boiler plate code.
    `npx create-react-app <Your Project Name Here>`
- After that go to the project folder and run the below command to start the development server (with the basic code got from the above command).
    `npm start`
- Now we can see the starting app in the browser and by default running in the port 3000.
- You can use the same settings with same IDE as we discussed for the NEXT JS in above section.

- NextJS is a framework, in that what we write is reactjs code.

## Data Fetching
   1. Static Generation
       - All the pages are pre-generated in advance in build time.
       - When we build the application for production, before we deploy it the production.
       - As Pages are prepared ahead to the time, they can be cached by the server/CDN serving the app.
       - The function used in the pages to prerender is,
            `export async function gerStaticProps(context){..}`
        - Should always return the object with the props key which will be returned to the component on that page.
        - The context parameter contains details of the application.
       - Any code we put in this function will never seen by the client side users/ in the browser.
       - You will not have access to standard client side APIs/objects like window in this function.
       - We can write any code that normally run on the server.(Means while building itself it is executed and static content is generated)
       - You can use the function for safe writing of some credentials here.
       - **Next JS pre-renders all the pages that have no dynamic data.**
       - It can't be used to the data that changes frequently. If you want to change the data generated in this function it need to be redeployed and server should start again.
       - To avoid this problem while using the static generation, nextjs provides a feature called **Incremental Static Generation**.
    
  1.1 **Incremental Static Generation:**
     - It prerenders the page.
     - By using this feature we can regenerate the page on every request atmost every X seconds while production(in the server side not in the browser).
     - That means We can serve old page if the regeneration is not needed yet/ not old yet. Or else we can,
     - Generate, store and serve "new" page which will replace the existing old page on the server. It will be cached and this regenerated page after X seconds can be seen by the future visitors.
     - To unlock this feature, we just need to return another key along with the props in the  `export async function gerStaticProps(context){..}` function which is **revalidate**. It takes no of seconds as input. 
     - getStaticProps function can return the object with the following keys:
        1. props - these will be passed to the component in that page.
        2. revalidate - No of seconds to re-render the page(until then the last rerendered page is shown.)
        3. notFound - It points to boolean value(true/false). If it is true 404 page will be rendered. By default it is false. It is mostly used in cases like when the data is not fetched or in other scenarios where we need to show the 404 page.
        4. redirect - We can redirect to another page instead of showing the current page.
     - getStaticProps function can accepts one parameter, called context. It can be named as you like but it specifically means context of application.
     context = {
        "params": [Means url params],
        }
   - But this context does not contain any request object.
     
   - If you have a dynamic page [params].js, by default the page is not pre-generated. Because nextjs dont know how many pages need to be prerendered by that page slug. So the staticProps will cause an error if we use in the dynamic pages.
   - Dynamic pages need to know which param values will be available for this js file, [param].js as multiple concrete page instances will be pre-generated for based on thr param values.
   - So for that, another export function is provided by next js in the page.
   - That is 
        `export async function getStaticPaths(){}`
   - It should also return an object as the getStaticProps does.
   - It returns the object with the following keys:
            1. paths: Its an array of objects which help nextjs to identify the pages that need to be pre-rendered directly in case of the dynamic route pages. Each object can contains,
                    -  params: {param:'<param_value>'}
            2. fallback: Suppose, if we took something like e-commerce page, if all the product detail pages are prerendered, it will not be good and it takes much long time to load all this pages which are not even opened sometimes.
                - fallback: false - Just the default option, to pre-render the pages.
                - fallback: true - The remaining pages that are not mentioned in the paths object are generated just in time.
           - So by returning these two keys, it allows us to pre-generate highly visited product pages by specifying them in the paths and setting fallback will load the page just in time.
           - But there will be a problem while using the fallback, if the user directly goes to that particular path it will not be loaded immediately so the props got from getstaticprops cause errors. Because this page is not pre-generated as we restricted with particular paths in paths key of the object returned by getStaticPaths as it takes *some time*.
          - We can overcome this in **two ways**. Using Fallback state or specifying fallback as blocking instead of true.
          - So, when we are using fallback feature, we should prepare a **fallback state** in our component.(Checking whether we got the required static props in to the component. If not just return other/loading component for mean time.) After we got the data it will be automatically rendered. 
          - **fallback:blocking** blocks loading the page directly until the data is loaded but it sometimes take long based on the content we load.
          - If we are using fallback and fallback state, when we are trying to access the page which is not there, we will get an error as static props cannot render the page. In such scenarios we also needs to check for that conditions and return the notFound as true from static props.(there comes the use of notFound key)
   
   2. Server-side Rendering
       - The pages are created just in time after deployment, when a request reaches the server.
       - It is used when we need to pre-render page for every request OR need access to request object.
       - So by using this, NextJs allows us to run Real Server Side Code as well.
       -    `export async function getServerSideProps(){}`
       -    Both server-side and  static props are used for the same purpose of returning props to the component but they will run at different point of times.
       - It also should return an object that should contain props key, may contain redirect and notFound key. But revalidate key cant be used as by default the serverside props will always run again for every request.
       - This also accepts a parameter called context and this context contains all that are available in the context of static props and also includes the req and res objects.

 ### useSWR
 - It is a react hook developed by nextjs community but it can be used in normal react projects also (but not on serverside).
 - This is a hook which underhood sends a http request using fetch API.
 - Stale-While-Revalidate (SWR) is a strategy to first return the data from cache(stale), then send the fetch request(revalidate) and finally come with the up-to-date data.
 - It provides the features like **automatic revalidation retries on error**.
 - `npm i swr`
 - useSWR requires typically atleast a URL of the request. 
 - Eg:
 ```
    const {data,error} = useSWR("url")
    if(!data)
        return <p>Loading...</p>
     if(error)
        return <p>Cannot load data..</p>
 ```

### _app.js
- It should be in/added in pages folder.
- It is a special next js file which allows us to set application wide settings.
- It can be treated something like root component inside of the body section of our HTML document.
- It is the main entry point of the nextjs application.

### _document.js
- It is should also be added in pages folder, if we want to use it.
- It allows us to customize the entire HTML document.
- All the HTML elements can be customized in the _document.js
- Here we need to add a special component, It must be class based component because it must extend some component offered and provided by nextjs.
- The component that we need to extend is Document component from next/document.
- We need to add a render method which returns some jsx element specific to the Document.
- All the components like HTML,Head, Main, NextScript from the nextjs should be imported and used in the class component that extends the document and in the _document.js.
- This document allows us to add attribute, tags or other directly on the html webpage.
- Main component is the used to render the nextjs components.
- So other than that we can add any tags outside of the nextjs components can be added here.
#### Default Structure of the JSX element returned in _document.js
- We need to return the jsx elements wrapped with HTML component in the render method.
- Then we have the Head component and body tag are in the HTML.
- Main component and Nextscript component can be used in the body tag.

### Optimizing Images
 - We can use the Image component from the next/image for optimizing the images instead of standard image element.
 - When we use this Image Component, next js will create multiple versions of our image on the fly.
 - When requests for the image are coming in, it optimize for the operating systems and device sizes that are making requests.
 - Later they are cached for future requests from similar devices.
 - These generated images are stored in .next/cache folder.
 - By default images are lazy loaded by using the Image component.
 - And it also done many background optimizations.
 
## API Routes
- Next js supports rest api routes.
- /api path URLs dont return pages(HTML) but instead behave as a REST API.
