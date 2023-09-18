1. Set Up the Environment
You will need to have a proper environment to work with Docker. Git and Docker are already installed and available in this Docker workspace. You will need to clone the BrezyWeather repository locally. The clone URL is available under the Documentation section.

2. Create the Dockerfile
You will need to create a Dockerfile for the BrezyWeather Web API project. You must place this file iside the labs-docker-dockerfile folder. For editing the code, you can use the in-built Vim editor. The Dockerfile should contain the instructions for building, publishing, and finalizing the source code into an image. The completed Dockerfile is available under the Assets section for reference.

3. Build the BrezyWeather Image
You need to create the BrezyWeather Docker image by building the Dockerfile you made earlier. Add a .dockerignore file to exclude the temporary folders, namely bin and obj. You need to tag the image using 1.0.0 to provide an explicit version of the image. This enables the developers to have a reliable version to use against. Verify the image presence once the build is complete.

4. Run the BrezyWeather Image to Create a Container
First, ensure the brezyweather image can run with the defaults. Next, you must create a Docker container instance for the brezyweather:1.0.0 image you created earlier. Name the container brezyweather-api and map host port 5000 to the Docker port 80. Finally, verify the container by executing GET /weather requests to fetch weather forecast details. For this, you can use the cURL command available within the terminal.

5. Clean Up the Resources
Please clean up the Docker containers and images created using appropriate docker commands. You must first stop the running containers and remove all the containers, followed by all the images.