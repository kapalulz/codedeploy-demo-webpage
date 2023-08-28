**Web Deployment with CodePipeline**

Project Overview:
This project focuses on setting up a Windows Server 2022 environment with a web server and automating the deployment process using AWS CodeDeploy and CodePipeline. The goal is to streamline the deployment of web applications hosted on the server whenever changes are pushed to a GitHub repository.

    Project Components:

1. Windows Server 2022 Setup:
  • Web Server: A web server has been installed on the Windows Server to host web applications.
2. AWS Roles Configuration:
  • EC2 Role.
  • CodeDeploy Role.
3. AWS CodeDeploy and CodePipeline:
4. YAML Configuration:

    version: 0.0
    os     : windows
    files:
      - source     : \
        destination: C:\inetpub\wwwroot

This configuration indicates that files from the source location (specified as \) will be deployed to C:\inetpub\wwwroot on the Windows Server.

    Workflow:
Developers push new code commits to the GitHub repository.
AWS CodePipeline detects the changes and initiates the deployment process.
AWS CodeDeploy uses the defined YAML configuration to transfer and deploy the updated code to the Windows Server 2022.
The web server on the Windows Server reflects the changes, making the updated application available to users.

    Benefits:
Automation: The project automates the deployment process, reducing the potential for human error and ensuring consistency.
Efficiency: Developers can easily and rapidly deploy updates to the web server.
Scalability: The setup can be scaled to handle more complex web applications and multiple servers.

    Conclusion:
This project successfully sets up a Windows Server 2022 environment, configures the necessary AWS roles, and implements a continuous deployment pipeline using CodePipeline and CodeDeploy. It offers an efficient and automated way to manage and deploy web applications hosted on the server, making it easier to deliver updates and improvements to end-users.


![image](https://github.com/kapalulz/codedeploy-demo-webpage/assets/17459523/67443504-02be-4b92-9221-15d9a56feb2f)
