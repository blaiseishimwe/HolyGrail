Inside index.js, function App we are referencing each of the components and we are 
passing onto each components both the function (handle) and the data. 
                              <Header  handle={handle} data={data}/>
the function Data simply displays the state of the data.
to fix the cross origin errors, run a little server. download http-server from node repository

                Steps
  1. Create a folder named public that will hold our Front end files
  2. In the root folder run npm init 
  3. create index.js
  4. Install Express
  5. use express to serve static files:
    app.use(express.static('piblic'));
  6. add async functions update() and read() for the    routes inside the front end index.js
  7. Add a database: Run Redis on Docker
      #docker image for Redis
      #This image expose includes Expose 6379 (the redis port)
      #so standard container linking will make it
       automativally available to the linked containers
$ docker run -p 6379:6379 --name some-redis -d redis

8. npm i redis

