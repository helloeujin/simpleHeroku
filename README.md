# Simple Heroku


### Getting started w/ local development server

Download and install Heroku Toolbelt <https://toolbelt.heroku.com>, this will give you Foreman and the Heroku CLI (command line interface).

1) Download this boilerplate repo and navigate into the code directory with Terminal.

2) Run **npm install** to get all required libraries.

	npm install

3) A Git repository and Heroku app are required for this Example to work. 

	git init
	git add .
	git commit -am "init commit"


4) Create Heroku app and add database

	heroku create 
	(for rename: heroku rename myApp)

7) Start server with **foreman start**.

	foreman start

Foreman reads your .env file, populates the process.env object for use in your app.

8) Open web browser to <http://localhost:5000> to view the web app.

9) Stop the web server press Command+C in the Terminal window.



### Local development server after installing

1) cd + drag folder directory

2) Start server with **foreman start**.

	foreman start
	
3) Push to heroku app
	
	git add .
	git commit -am 'edit'
	git push heroku master
	
	(git push origin master // for github update)
	
4) Open heroku app

	heroku open


### Frameworks and NodeJS

Libraries and frameworks are created for all programming languages to make complicated programming tasks more easier to program. A database library will create the connection to the database server, insert and query data and return a result that is easily used. A framework involves the same ideas of a library but it usually is larger in size and complexity - picking a framework is usually done at the beginning of development because it is often difficult to switch to another. Android, Arduino, OpenFrameworks, Sinatra, Ruby on Rails, Django and Processing are frameworks, each is a collection of libraries to interact with lower level code.

Libraries and frameworks are available to make your programming life easier - someone else has had similar tasks and requirements so they organized their code into a library and made it available to the community.

#### ExpressJS

ExpressJS (http://expressjs.com/guide.html) is a popular framework for building web applications in NodeJS. ExpressJS's core is taken from the Connect framework.

#### Routing

Routing is how you direct the user's requested URL to retrieve the appropriate 'page' or save the submitted form. All routes execute functions, the callbacks should receive a request and response object from Express

app.get('/page1',function(request, response){
    //your code goes here
})

#### HTTP Methods

GET- a user requests a web page or resource

	app.get('/about',function(request, response){
	    console.log("GET request for /about");
	    response.send("This is the about page.");
	});

-----

More about Express.js (https://github.com/johnschimmel/Heroku-ExpressJS-Boilerplate)
