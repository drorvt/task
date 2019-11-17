In this article we will see how to create a simple continuous integration process using Github, Travis-CI and Docker HUB

App
We will review the docker file, the app code and the travis-ci file, so let’s start with the app main.go:

Docker
Travis
Putting everything together
So far we got the repo going, the configuration for travis, the dockerfile, the app, but now we need to make use of it, so you will need to create a travis account for this to work then link your github account to it, then you will be able to sync your repositories and you should see something like this:
Once you have your account linked you will be able to sync and enable repositories to be built.
After enabling the repository you can configure some details like environment variables, here we will set the credentials for dockerhub.


After the repository is created we can trigger a build from travis or push a commit to the repo in order to trigger a build and to validate that everything works.
You should see something like this in travis if everything went well:


You can validate that everything went well by checking the commit SHA that triggered the build.
And dockerhub:
