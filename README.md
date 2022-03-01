# Router Assignment

In this assignment we will use React Router to create a single page application where we can route to different pages.

## Task 1 Setting up
Open the terminal and do the following:
 - `npm i` to install the node modules. 
> notice in `package.json` that the `react-router-dom` module was also installed. 


## Task 2 Create a new folder structure
Open the `src` folder and create the following folder structure: 
 - components
 - routes 
 
 ## Task 3 Enable the router inside the Application
 
 ### Task 3.1 import the router functionality.
 Import the following items from `react-router-dom`
 ```javascript
  import { BrowserRouter, Routes, Route } from "react-router-dom";
 ```

  ### Task 3.2 Add the router tags the the render function
  Add in the following inside the render function of `App.js`.
   ```javascript
    <BrowserRouter>
        <Routes>
        </Routes>
    </BrowserRouter>
```
 
## Task 4 Adding in pages for our Routes. 
In this taks we want to create our page components.

### Task 4.1 Creating pages
Navigate to the `routes` folder and create the following folders:
- HomePage
- AboutPage

Make sure that each folder contains the corresponding component file. Inside HomePage this will be `HomePage.js` and inside AboutPage this will be `AboutPage.js`.

result should be: 
- HomePage
  - `HomePage.js` 
- AboutPage
  - `AboutPage.js` 


 ### Task 4.2 Creating page components
 Create for each page, a component use the following snippet as an example to create the component: 
```javascript
export default function Homepage() {
  return (
      <div>
         <h1>I am a page component</h1>
      </div>
  );
}
```

## Task 5 Wiring up the routes. 

### Task 5.1 Importing the pages.
Open `App.js` and import the two page components: 

Example: 
```javascript
import Homepage from "./routes/Homepage/Homepage";
```

### Task 5.2 Creating the routes.
Inside `App.js` add two new routes inside the `<Routes>` tag.  
One route should have `path="/"`to the root of the application and the othe should be accessible through `/about` so the path should be `path="/about"`.

Snippet for a route: 
```javascript
 <Route path="/" element={<Homepage />} />
```
### Task 5.3 Start the application and test.
Run `npm start` in the terminal and test by navigating to the about page (`/about`) and to the homepage (`/`). In each case you should see their corresponding page component.

