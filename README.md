## Simple Typescript application with Vite

This is a template project to quickly create a Typescript application with Vite.

# Quick Start

- Create a new Github repository using this repository as template
- Clone your new repository
- Copy the `./code/.env.example` file to a `./code/.env` file
- Edit the content of the `.env` file to match your preferences (see next section for details)
- Run the following commands:

```
make setup
make dev
```

If you don't have `make` on your machine, simply run:

```
./etc/bin/setup.sh
./etc/bin/dev.sh
```

Your application will be running on http://localhost:5173

## Environment

Here are the current environment variables to set in the `.env` file:

- VITE_APP_NAME: set the name of your application. It will be the `<title>` of the webpage and used in some logging
- VITE_APP_VERSION: the version of the application. It gets overwritten when you build your docker image in Github Actions.
- VITE_FACEBOOK_APP_ID: if you have a Facebook App associated with this application. Otherwise remove from the `index.html` file
- VITE_DESCRIPTION: the description of the application, used in the meta tags for SEO
- VITE_APP_URL: the URL where this application is running, used in the meta tags for SEO
- VITE_APP_IMAGE: the marketing image to use, used in the meta tags for SEO
