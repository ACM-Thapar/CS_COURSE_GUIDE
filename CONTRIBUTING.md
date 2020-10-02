# Welcome to the contributions of OPTIM

We follow a systematic Git Workflow -

- Create a fork of this repo.
- Clone your fork of your repo on your pc.
- [Add Upstream to your clone](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/configuring-a-remote-for-a-fork)
- **Every change** that you do, it has to be on a branch. Commits on master would directly be closed.
- Make sure that before you create a new branch for new changes,[syncing with upstream](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/syncing-a-fork) is neccesary.

## Setup and running of project (Backend)

- Fork the repo and clone it.
- If you had a previous version of the project, please delete the old env folder and create a new one
- The project now uses node.js , you should have a node version greater than 12.0.0 to run the project

- You should have pre-commit installed , do it using the command<br> `curl https://pre-commit.com/install-local.py | python -`

- Run these commands

```bash
pre-commit install
```

- This will setup the project requirements and pre-commit test hooks!

- Setup a test databse on mongodb Atlas
- Create a user , establish the network connection on mongo db atlas
- Create a new cluster.

- change the current directory and navigate into the server folder using the command <br> `cd server`
- Copy the connection url of the databse and paste it in the ./server/.env file and doker-compose.yml file .

- To install all the dependencies run 'npm i'

- Setup the .env file using the instruction in the section below

- After the above setup, run <br>
  `nodemon .` or
  `node .`

- This will start the backend dev server
  Runs the backend server at default port `5000`.<br />
  Open [http://localhost:5000](http://localhost:5000) to view it in the browser.

- To exit the poetry virtual environment run `exit`.

## Setting up the ./server/.env file

- create a .env file in the server directory
  -the ENVIRONMENT VARIABLES REQUIRED ARE --<br>
  GOOGLE_CLIENTID = ' ' <br>
  GOOGLE_CLIENTSECRET <br>
  MONGO_URI <br>
  COOKIEKEY = 'any random value' <br>
  JWTTOKEN = 'any random value<br>
  GITHUB_CLIENTID = ' setup a github o-auth application and copy this ' <br>
  GITHUB_CLIENT_SECRET = ' setup a github o-auth application and copy this '<br>
  UPLOAD_DP = ' folder id of a drive folder '<br>
  UPLOAD_POST = ' folder id of a drive folder '<br>

## Setup and running of project (Frontend)

- navigate into the client directory using <br> `cd client`
- At your client directory run `npm install` to install all the dependencies
- Start react dev server
- `npm run start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

## Running with Docker (Backend)

- Ensure that you have `docker` and `docker-compose` already installed.
- At the root of the project directory run `docker-compose up --build` to build the image for the first time.
- To start the backend run `docker-compose up -d`.
- Ensure that the backend is running by going to [http://127.0.0.1:4000](http://127.0.0.1:4000).

## Generating a CLIENT ID for Google OAuth Login

- Create a new project with name **OPTIM** in _Google Cloud Platform_.
- Enable **Cloud OS Login API** from the API Library in _Google Cloud Platform_.
- Go to **API & Services** section and click on **Create Credential**.
- Choose _OAuth Client ID_.
- Setup the consent screen if asked to do so.
- Select **Web Application** as the _Application Type_.
- Whitelist `localhost:3000` under _Authorised Javascript Origins_.
- Click on **Create**
- Copy the **ClientID** and paste it in `.env` file alongside **REACT_APP_OAUTH_CLIENT_ID**.

## Using Google Cloud Storage for storing _static_ and _media_ files (Only required for PRODUCTION)

- First, you need a service account for connecting to GCP
- Head over to this [page](https://cloud.google.com/docs/authentication/getting-started) and click on **Create Service Account**
- Select the relavant project
- From the dropdown for _Service Account_ choose _New-service account_
- Download the `JSON` file and store it at your project root.
- Rename the file to `service-account.json`
- Set `GOOGLE_APPLICATION_CREDENTIALS` to the path to `service-account.json` in above point in the `.env` file.
- Create a bucket on GCP with the relavant name
- Copy the bucket name and in `.env` file set `GS_BUCKET_NAME` to your bucket name.

#### Note

- As the project now uses `npm` to manage dependencies, you need to run `npm install <package_name>` **IN THE SERVER OR CLIENT RESPECTIVELY** to install the new package.
