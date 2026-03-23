# Streamline-Your-Static-Website-Deployment-Craft-a-Seamless-CI-CD-Pipeline-with-AWS-CodePipeline
Set up an automated deployment pipeline for a static website leveraging AWS services. This CI/CD pipeline, powered by AWS CodePipeline, will automatically trigger whenever changes are made to the website’s code in a connected GitHub repository
![1_lFUDCO09rYnEqdRLJ9SUXA](https://github.com/user-attachments/assets/c08edae0-7a22-4829-94b3-f9b0b0000e72)

Development team is bogged down by manual website deployments. Each update involves a cumbersome, time-consuming process that slows your release cycle and increases the likelihood of errors. Fortunately, there’s a better way: CI/CD (Continuous Integration and Continuous Delivery). In this guide, we’ll show you how to transform your workflow from tedious manual steps to seamless automation using AWS CodePipeline.

Our goal is to set up an automated deployment pipeline for a static website leveraging AWS services. This CI/CD pipeline, powered by AWS CodePipeline, will automatically trigger whenever changes are made to the website’s code in a connected GitHub repository.

How It Works

We’ll start by creating a new GitHub repository and uploading the website’s HTML files. Next, an S3 bucket will be set up to host the website. Finally, we’ll configure AWS CodePipeline to connect the GitHub repository with the S3 bucket. With this setup, any changes pushed to the GitHub repository will trigger the pipeline, automatically building and deploying the updated website to the S3 bucket. This automated process ensures your website stays up to date with minimal effort — just push your code, and the rest is handled for you!

Let’s dive in and get started!

Step 1: Create a Repository in GitHub and upload HTML file in

In this article, I’m committing changes directly to the main branch for simplicity. However, in a real-world scenario, this approach is not recommended. Developers should work on a separate branch, thoroughly test their code, and only merge it into the main branch after
ensuring its stability.

 ![1_fMyFWN-iz-ZUeOGfxvb2gw](https://github.com/user-attachments/assets/d1319f3d-f1d6-44da-86fd-71c010526567)
