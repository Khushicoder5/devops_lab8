# Lab 8: Jenkins Hello World Job

## Objective
To create and execute a Jenkins Freestyle job that retrieves a shell script from GitHub and displays a Hello World message.

## Tools Used
- Jenkins
- Git and GitHub
- Shell scripting

## GitHub Repository
[devops_lab8](https://github.com/Khushicoder5/devops_lab8)

## Jenkins Localhost URLs
- **Jenkins Dashboard:** http://localhost:8080/
- **HelloWorld Job:** http://localhost:8080/job/HelloWorld/
- **Build #1 Console Output:** http://localhost:8080/job/HelloWorld/1/console

## Script: hello-world.sh
```bash
#!/bin/bash
echo "Hello, Jenkins!"
```

## Jenkins Configuration
- **Job Name:** HelloWorld
- **Job Type:** Freestyle project
- **Source Code Management:** Git
- **Branch:** main
- **Build Command:** `sh hello-world.sh`
- **Repository URL:** https://github.com/Khushicoder5/devops_lab8.git

## Expected Console Output
```text
Hello, Jenkins!
Finished: SUCCESS
```

## Result
Successfully created and executed the Jenkins Hello World job. Jenkins cloned the GitHub repository, executed the shell script, and displayed the expected output.

## Note
The localhost URLs are accessible only on the local machine where Jenkins is running and while the Jenkins service is available.