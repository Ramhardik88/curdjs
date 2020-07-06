# curdjs
Disclaimer: Understanding of JavaScript, MongoDB, HTML and CSS | Full-Stack Web Development is a pre-requisite.

CRUD (Create, Read, Update and Delete) Application in NodeJS

Node.js is a JavaScript library to write server-side scripts.
Before it, JavaScript was used for client side script to run on browser, but Node.js enabled us to write server-side scripts running on server to delivery dynamic web pages to client's browser.

TERMINOLOGIES & INSTALLATION

Follow through following installation instruction and terminologies to understand how the code attached with this git or to create your own application in Node.

    Download and Install Node.js from Download Node.js.

    After installing Node.js navigate to your project directory and run following commands in terminal to initialize project:


    			npm init
    		

    Running above command will ask you few question - enter project name and press enter for all. You will find package.json file, open it in editor and replace following line to set Node start command and specify start page:


    			"test": "echo \"error..."
    		

    to


    			"start": "node index"
    		

    Next, create a blank index.js file in the same directory. This is the start page.

    Now, you can run your Node.js application by running following commands in terminal:


    			node start
    		

    However, we are going to use nodemon to run Node.js application. Install by running following command:


    			npm install -g nodemon
    		

    Now you can start your application with command: nodemon. The beauty is that the code will be auto-compiled and executed after saving, saving you the hassle of restarting the server every time you modify your code as in case of start node.

    Express is a Node.js framework that simplifies the work of Node.js. Read about it from: Express.js.

    Run following commands to install express framework:


    			npm install --save express
    		


    Pug is a template engine used instead of HTML. Read about it from: Pug.js

    Run following commands to install pug template engine:


    			npm install --save pug
    		

    Note: You can choose to convert HTML to Pug from HTML2Jade (html2jade.org). Pug was originally known as Jade.

    Mongoose is a npm package for MongoDB object modeling designed to work asynchronously. Read about it from: Mongoose

    Run following commands to install mongoose package:


    			npm install --save mongoose
    		

    Obviously, you need to have MongoDB installed and set up a database 'nodejs_crud_app'. You can download and install from: MongoDB.

    Body Parser is npm package used to parse input form body in desired format. However, we will parse in JSON.

    Run following commands to install body parser package:


    			npm install --save body-parser
    		


    Bower is a package manager like npm for installing packages like bootstrap, jquery, etc.

    Run following commands to install Bower package manager:


    			npm install -g bower
    		

    Note: We need to setup a installation for bower. To do so create a file called .bower.rc (note the '.') and put following line into it:


    			{"directory":"public/bower_component"}
    		

    We will not use it. But, it's good that you know it for building real-life applications.

    We will also need express-messages and connect-flash for flash message, express-session for user session and express-validator for validation. Install all using following command:


    			npm install --save express-message express-session connect-flash express-validation
    		

    Follow through all of their documentation online.

    Lastly, we will use passport for authentication. Read about it from : passportjs.org.

    Run following command to install passport authentication manager:


    			npm install --save passport passport-local bcryptjs
    		

    Above, passport-local is used to interact with local storage like MongoDB and bcrypt for encrypting passport.



LET'S WRITE THE CURD APP IN NODE JS

I prefer the hard way, therefore, I am not going to explain you everything over here, but I will make sure that the code have enough documentation to explain you everything.

Download and Run Code:

Download the code from this git repository and follow through all the code comments.

To run the downloaded code navigate to project directory in terminal and run command: nodemon and visit http://localhost:3000/ in browser to see app running.
