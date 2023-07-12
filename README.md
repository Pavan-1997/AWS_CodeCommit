# AWS CodeCommit

AWS provides a comprehensive set of CI/CD (Continuous Integration/Continuous Deployment) services that enable developers to automate and streamline their software delivery processes. They are AWS CodePipeline, AWS CodeBuild, and AWS CodeDeploy are the key services 
involved in achieving CI/CD on AWS platform. 

![image](https://github.com/Pavan-1997/AWS_CodeCommit/assets/32020205/b0809130-cdeb-420a-9b43-2bb0a81c2757)

It is similar to private repositories like GitHub Enterprise and GitLab used in organizations.
 
Advantages of CodeCommit:

- Managed Git
- Scalability
- Reliablity


Disadvantages of CodeCommit:

- Features
- AWS Restricted
- Fewer integrations with services outside AWS

---
# Using AWS CodeCommit - Cloning - Commit - Push to Remote Repo

1. Goto AWS Console and search for Code Commit 

2. Now click on Create repository

Give name to it

Give description

No need to select the AWS Code Guru which is specific to JAVA and Python

Now click on create buttun 

Now upload any file into it using UI 

We can push file to Code Commit using UI or cmd (using UI we can commit only one file hence using cmd)


3. AWS recommends to use devops tools using a IAM account bit not root account

Goto IAM -> Give a User name -> Check Provide user access to the AWS Management Console -> Select I want to create an IAM user -> Give a custom password -> You can uncheck the User must create a new password at next sign-in -> Click on Next -> Click on Attach policies directly -> Select AWSCodeCommitPowerUser -> Click on Next and  Create user

4. Now login to AWS console using the IAM user and access the repo that you have created and see the file inside the repo

5. Access the repo from the local terminal (Preq: Make sure you have Git already installed in it)

Now go the repo -> Click on Clone URL -> Click on Clone HTTPS -> Goto the local terminal(GitBash) and use the below

git clone <Clone-HTTPS>

6. Goto the directory and see the file in the repo

7. Create a file in the repo say below

touch test.txt

8. Add the file created to staging area

git add test.txt

9. Commit the file 

git commit -m "Test"

10. Push the file to the remote AWS repo 

git push origin master




 
