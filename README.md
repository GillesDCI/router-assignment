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
