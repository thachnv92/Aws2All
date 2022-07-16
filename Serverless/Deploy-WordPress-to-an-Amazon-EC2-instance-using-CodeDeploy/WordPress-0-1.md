# <center>0.1. Install or upgrade the AWS CLI on Engineer machine</center>

# Guide
To call CodeDeploy commands from the AWS CLI on a local development machine, you must install the AWS CLI. CodeDeploy commands first became available in version 1.6.1 of the AWS CLI. CodeDeploy commands for working with on-premises instances became available in 1.7.19 of the AWS CLI.

If you have an older version of the AWS CLI installed, you must upgrade it so the CodeDeploy commands are available. Call `aws --version` to check the version.


For installation instructions, expand the section for your operating system to install or upgrade the AWS CLI.

## **Linux**
<details>
  <summary>Expand</summary>

## Installation requirements
- You must be able to extract or "`unzip`" the downloaded package. If your operating - system doesn't have the built-in unzip command, use an equivalent.
- The AWS CLI uses `glibc`, g`roff, and `less`. These are included by default in most major - distributions of Linux.
- We support the AWS CLI on 64-bit versions of recent distributions of CentOS, Fedora, Ubuntu, Amazon Linux 1, Amazon Linux 2 and Linux ARM.
  
## Install or Upgrade the AWS CLI
```
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```

## Confirm the installation with the following command
```
which aws
aws --version
```

</details>

## **macOS**
<details>
  <summary>Expand</summary>

## Installation requirements
- We support the AWS CLI on Apple-supported versions of 64-bit macOS.
- Because AWS doesn't maintain third-party repositories, we can’t guarantee that they contain the latest version of the AWS CLI.
  
## Install or Upgrade the AWS CLI
```
curl "https://awscli.amazonaws.com/AWSCLIV2.pkg" -o "AWSCLIV2.pkg"
sudo installer -pkg AWSCLIV2.pkg -target /
```

## Confirm the installation with the following command
```
which aws
aws --version
```

</details>

## **Windows**
<details>
  <summary>Expand</summary>

## Installation requirements
- We support the AWS CLI on Microsoft-supported versions of 64-bit Windows.
- Admin rights to install software
  
## Install or Upgrade the AWS CLI
Download and run the AWS CLI MSI installer for Windows (64-bit):
https://awscli.amazonaws.com/AWSCLIV2.msi.

Alternatively, you can run the msiexec command to run the MSI installer.
```
msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi
```

## Confirm the installation with the following command
```
aws --version
```

</details>

***

For more detail, follow this [AWS page](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html).
 
***


Next page: [Configure the AWS CLI on Engineer machine](WordPress-0-2.md)