# Assignment
  My name is Piyush Gupta and I have completed the assignment as it was required. 
  
  To run the application in your computer do the following steps:
  1. Clone the repository in your computer.
  2. Run npm/yarn install in reactjs and server folder to download all the dependencies.
  3. In conn.js, change the DB variable to your local mongoDB.
  4. Change the PORT in app.js to 5000.
  5. In userSchema.js on line 85, change process.env.SECRET_KEY to 'thisisiriatechinnovationsandtechnologypvtltd'(or anything greater than 32 characters)
  6. Run node app.js in server, and npm start in reactjs folder simultaneously.
  
  The details of the files in the repo are as follows:
  There are two folders named server and Reactjs.The server folder contains all the backend part including database.The Reactjs contains all the frontend part.
  The elements of the frontend are done using bootstrap.You can see the dependencies used in package.json file in both server and Reactjs folder.
  The backend is running at localhost:5000 whereas the frontend is running at localhost:3000. The frontend and backend are connected by adding 
  "proxy": "http://localhost:5000/" in package.json file of Reactjs folder.
  
  Contents in Server folder:
  1: db: The db folder contains conn.js which is used to connect to mongoDB atlas cluster or the local mongoDB server.
  2: middleware: The middleware folder contains authenticate.js which ensures that the user cannot visit aboutus page unless he is signed in using jsonwebtokens(jwt).
  3: model: The model folder contains userSchema.js which defines the schema of the database.Password hashing and assigning jwt token is also done here.
  4: router: The router folder contains auth.js which handles all the routings.
  5: app.js: The backend server runs through app.js at post 5000.
  
  Contents in Reactjs folder: 
  1: public: The public folder mainly contains index.html which only contains the one div element.
  2: src:
    components: The components folder contains all the pages used such as Home page,user profile(about) page,sign in page,sign out page.
                Bootstrap is used to design all the pages and react hooks are used to route the pages.
    reducer: The reducer folder contains useReducer.js which is used to store and update states instead of using useState.
    images: All the images used in the project are stored here.
    app.js: The user is rerouted to the page he requested in app.js
    app.css: Css used in all components is written here.
    index.js: The contents of app.js are rendered to index.html using index.js
    
