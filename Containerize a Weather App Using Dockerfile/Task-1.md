# Task-1
My team is using a Dockerfile to containerize a .NET API app. 
However, the manager is concerned about the image size being 1.5 GB. 
This higher image size has led to performance issues during the build process and at production. 
I'm expected to optimize the image using best practices in building a Docker image. 
I must split the Dockerfile build into multiple stages to form a layered approach to 
building the image. Also, I need to use .NET Runtime for the final stage of the image instead 
of the existing .NET SDK image. Finally, I must build and compare the image size with
the original to ensure the final image is optimized.