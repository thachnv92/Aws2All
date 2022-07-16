# <center>1. Launch and configure an Amazon Linux</center>

# Guide
To deploy the WordPress application with CodeDeploy, you'll need an Amazon EC2 instance running Amazon Linux. The Amazon EC2 instance requires a new inbound security rule that allows HTTP connections. This rule is needed in order to view the WordPress page in a browser after it is successfully deployed.

Follow the instructions in Create an Amazon EC2 instance for CodeDeploy. When you get to the part in those instructions about assigning an Amazon EC2 instance tag to the instance, be sure to specify the tag key of Name and the tag value of CodeDeployDemo. (If you specify a different tag key or tag value, then the instructions in [Step 4: Deploy your WordPress application](WordPress-4-0.md) may produce unexpected results.)

# Tasks:
1. [Launch an Amazon EC2 instance](WordPress-1-1.md)
2. [Install the CodeDeploy agent for Amazon Linux](WordPress-1-2.md)

***


Next page: [Launch an Amazon EC2 instance](WordPress-1-1.md)