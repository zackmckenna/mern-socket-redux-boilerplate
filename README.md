This is a Boilerplate for a MERN stack application, with basic user authentication, database modeling and log in on the front-end. Includes Redux integration with socket.io which allows the dispatch of actions between the clients Redux store and clients socket. Users can dynamically create, join, leave and message rooms.

## Available Scripts

In the skeleton-card-react project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

In the skeleton-card-server project directory, you can run:

### `yarn run watch`

Launches the server in watch mode, which causes the server to reload if you make any edits.

### `yarn run build:ui`

Removes any current build in the back-end directory, creates a new build in the front end and copies it to the back-end for deployment.

To connect to you MongoDB, create a file called .env in the skeleton-card-server project directory, and add:

MONGODB_URI=**YOUR_MONGO_DB_CONNECTION_STRING_HERE**

Make sure .env is in your .gitignore

To deploy on Heroku, look up Heroku documentation to set up Heroku CLI and run heroku create in the skeleton-card-server directory.

In the newly-created Heroku project, you'll have to add the MONGODB_URI from your ..env file to the Heroku projects configs.

Then, run:

### `yarn run build:full`

Runs the build command above then deploys the entire application to Heroku.
