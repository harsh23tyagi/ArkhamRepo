-- This is a standardize bundle for a kickoff project of flask--
Anyone can use this bundle for creating the first flask application and then run it locally
--Currently this bundle does not includ deployment to the web server on cloud, but in future build it will also be included--

---------------------------------------------------------------------------------------------------------------------------------------

Folder Description:
cli/commands: Used for creating cli commands shorter, especially for coverage and tests
config: contains runtime configuration for development phase
instance: contains runtime configuration for production phase
Portal: Everything that is required as the content or module for your flask application is inside this folder
blueprints: Contains all the html files which can be used as blueprint in application (Know more about blueprints from documentation)
static: Contains all the static files such as fonts, images, styles and scripts
templates/layout: Contains app specific html templates or contains html templates which are derived from the templates made in blueprints section
tests: Test related content


---------------------------------------------------------------------------------------------------------------------------------------

File Description:
cli.py: Calls the command files in the commands folder
settings.py: contains configuration
app.py: Kick off flask file to contemplate the views and project on screen hosted on a server locally
_env: (Type is not required) Contains the name of the Content folder for the docker file (e.g. in this case the name is 'Portal')
docker-compose.yml: Helps in maintaining our deployments in docker-compose
Dockerfile: (Type is not required) Helps in maintaining our deplioyments in dockers
requirements.txt: Dockerfile runs this file to install all requisites for the app. Any more external libraries if required can be added in this file
setup.py: A setup file for cli
---------------------------------------------------------------------------------------------------------------------------------------
How to run the project?

install docker in your system- (linux or mac recommended. If on windows use docker quickstart terminal)

-> Open terminale
-> write the following command:
docker-compose up --build (Prefix command with sudo if on linux)

Open your browser and type in url bar:
localhost:8000

