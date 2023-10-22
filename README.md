<h1>Automated AWS CICD Pipeline for EC2 Web Hosting with GitHub Actions</h1>

<h2>Description</h2>
This GitHub repository is a complete demonstration of a seamless Continuous Integration and Continuous Deployment (CICD) pipeline for hosting a website on an AWS EC2 instance using GitHub Actions. With this project, you'll learn how to automatically update and redeploy your website whenever there's a new commit to the main branch. The repository includes detailed instructions, configuration files, and sample code to help you set up this CICD process for your AWS-hosted website.<br />
Whether you're a developer, DevOps engineer, or just looking to automate your deployment process, this repository will be your go-to resource for building a robust and automated CICD pipeline for your AWS-hosted website. Streamline your development workflow and keep your website up-to-date with every code change.
<br />

<h2>Services Used</h2>

- <b>AWS Elastic Compute Cloud(EC2)</b>
- <b>GitHub Actions</b>

<h2>Project Walkthrough:</h2>

<p align="center">
Log into AWS console, find the AWS EC2 and create an EC2 instance as shown, save your EC2 session key: <br/>
[<img src="https://i.imgur.com/tCK3KvC.png" height="80%" width="80%" alt="Project Steps"/>]
[<img src="https://i.imgur.com/SC1vAeI.png" height="80%" width="80%" alt="Project Steps"/>]
[<img src="https://i.imgur.com/y2Z0ahs.png" height="80%" width="80%" alt="Project Steps"/>]
[<img src="https://i.imgur.com/jFTBWhK.png" height="80%" width="80%" alt="Project Steps"/>]

<br />
<br />
Wait for the EC2 instance to launch and finish the necessary checks:  <br />
<img src="https://i.imgur.com/XClTV4M.png" height="80%" width="80%" alt="Project Steps"/>

<br />
<br />
Create a GitHub repository for the deployment and upload your website code: <br/>
<img src="https://i.imgur.com/NC93rEN.png" height="80%" width="80%" alt="Project Steps"/>
<br />
<br />
Go to the GitHub actions and set the secret variables for the GitHub to interact EC2 instance:  <br/>
<img src="https://i.imgur.com/QBaOkRG.png" height="80%" width="80%" alt="Project Steps"/>
<img src="https://i.imgur.com/ttBnAOG.png" height="80%" width="80%" alt="Project Steps"/>
<img src="https://i.imgur.com/XMDL6jQ.png" height="80%" width="80%" alt="Project Steps"/>
<img src="https://i.imgur.com/LygKlVx.png" height="80%" width="80%" alt="Project Steps"/>
<img src="https://i.imgur.com/8e9mLVp.png" height="80%" width="80%" alt="Project Steps"/>

<br />
<br />
Go to .github/workflows and create a file "github-action-ec2.yml" as shown:  <br/>
<img src="https://i.imgur.com/EgFjiQK.png" height="80%" width="80%" alt="Project Steps"/>

<br />
<br />
Wait for your GitHub workflow to deploy the website on the EC2 instance, access the website through the ipv4 address of the instance:  <br/>
<img src="https://i.imgur.com/6qwE0ks.png" height="80%" width="80%" alt="Project Steps"/>
<img src="https://i.imgur.com/zI5hy7E.png" height="80%" width="80%" alt="Project Steps"/>
<img src="https://i.imgur.com/KTJVxba.png" height="80%" width="80%" alt="Project Steps"/>
<br />
<br />
We can verify the CI/CD pipeline by changing the website code and committing the changes to the main branch of repo:  <br/>
<img src="https://i.imgur.com/K84M2XD.png" height="80%" width="80%" alt="Project Steps"/>
<br />
<br />
Wait for the redeployment to be finished, to see your redeployed website:  <br/>
<img src="https://i.imgur.com/LR6Xz6M.png" height="80%" width="80%" alt="Project Steps"/>
<img src="https://i.imgur.com/GVB8712.png" height="80%" width="80%" alt="Project Steps"/>
<img src="https://i.imgur.com/chHOfLJ.png" height="80%" width="80%" alt="Project Steps"/>

</p>
<p><ins>NOTE:</ins> The instance in the above example is terminated due to security reasons.</p>

<h2>Conclusion:</h2>
In conclusion, this GitHub repository showcases a practical and efficient way to implement Continuous Integration and Continuous Deployment (CICD) for hosting your website on an AWS EC2 instance. By following the provided instructions and using GitHub Actions, you can seamlessly automate the deployment process, ensuring that your website remains up-to-date with every main branch commit.
<br />
This project illustrates the synergy between popular development tools and AWS services, offering a valuable solution for developers and teams aiming to streamline their deployment workflow. It empowers you to harness the capabilities of AWS and GitHub for a more efficient and automated web hosting process, saving time and effort.
<br />
By utilizing this repository as a reference, you can enhance your understanding of CICD practices, AWS integration, and GitHub Actions, ultimately benefiting your projects and ensuring your website's continuous availability. Take advantage of this resource to keep your web content current and effortlessly deploy updates with confidence.
