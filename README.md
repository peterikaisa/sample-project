# A small, general, sample project for prototyping

Sample project created with `vue create` from [Vue CLI](https://cli.vuejs.org/). Currently has the simplest, non-safe markdown editor. Maybe I'll sanitize it one day, if I have the time...

This repo is published into [Docker Hub] and deployed (manually) to https://sample-project-k.herokuapp.com/.

## Running locally

Setup repository with `npm install`, then run a dev server with `npm run serve`. Build for production with `npm run build`. Serves from port `8080` on default.

### Running in Docker

Includes two (2) Dockerfiles (and nginx confs), one tailored spesifically for deploying to [heroku] (Thanks, I f- owe you a beer, sis) and one for running in local containers (where one can publish their own ports). CircleCI deploys from `Dockerfile` on default, so you can build your local image from `Dockerfile.local` and then run it with `-p 8080:80`.

[heroku]: https://dev.to/levelupkoodarit/deploying-containerized-nginx-to-heroku-how-hard-can-it-be-3g14
[Docker Hub]: https://hub.docker.com/repository/docker/peterikaisa/sample-project