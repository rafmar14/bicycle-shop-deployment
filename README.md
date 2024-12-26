# bicycle-shop-deployment

Project with the goal to automate the build, test, configuration and deployment of the docker images for the main environments. Every project has a dockerfile that will create the image and a docker-compose that will coordinate every container:
- Proxy NGINX: Entrypoint that handles the requests and redirect to the the container.
- Backend: Container that runs the server app
- Frontend: Container that runs the client app

The CI/CD platform will be Github actions that has a free feature for public repositories and will be deployed to Render, a cloud application platform that supports docker containers.