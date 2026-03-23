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

Step 2: Create and Configure an S3 Bucket :

*Make sure static website hosting is Enabled
*Block all public access should be turned OFF
*Also update bucket policy accordingly .
*Upload your HTML file

![1_nYR76p8dM4q8fAoEPyX1RQ](https://github.com/user-attachments/assets/dbf7e5f7-b026-4560-a56f-3fadeecb702d)

Step 3: Create a CI/CD Pipeline Using AWS CodePipeline

*Go to the CodePipeline service. Click Create pipeline and Enter a pipeline name: CDA06pipelineTW.
*For the Source Stage .Select “GitHub (app version)” as the source provider.
*Connect to GitHub and authorize AWS CodePipeline to access your repository.
*Select the repository and branch (main)
*Skip the Build Stage by clicking Skip build stage and then Skip.
*For the Deploy Stage .Select “Amazon S3” as the deployment provider.
*Select your bucket: cicd-luit-project
*Review the settings and click “Create pipeline.”

![1_-CxcjQ7jmQ_k3-YLvRtEDQ](https://github.com/user-attachments/assets/afe2b039-aad9-4bc3-a087-a0fff50b24ce)

Step 4: Verify and Update the Pipeline

Make an update to the code in your GitHub repository and commit changes .
The CodePipeline should automatically trigger upon this change

If you found it helpful, don’t forget to show some love with a thumbs up — let’s get to it! 🙌
