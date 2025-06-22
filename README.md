**🚀 Automation Setup for Nexus, Jenkins, SonarQube, and Docker 🛠️**

This script automates the setup of Nexus, Jenkins, SonarQube, and Docker on an Ubuntu server. It creates users, installs dependencies, configures the software, and ensures services are up and running. The script also ensures these services are set up to run on system startup for persistence.

**📝 Steps Automated by the Script:**

**1. Nexus Setup 🔧**
Nexus is a repository manager that helps manage your software artifacts. The script automates its installation and configuration.

Create Nexus User: Adds a user named nexus for secure access.

Install OpenJDK 17: Necessary for running Nexus.

Download & Install Nexus: Downloads the latest version of Nexus, extracts it, and configures the necessary permissions.

Service Configuration: Nexus is set up to run as a service using systemd.

**2. Jenkins Setup 🤖**
Jenkins is a popular open-source automation server for continuous integration and delivery.

Add Jenkins Repository: Adds Jenkins’s repository and key to the system.

Install Jenkins: Installs the Jenkins package.

Service Configuration: Jenkins is set up to run as a service, ensuring it starts with the system.

**3. SonarQube Setup 🔍**
SonarQube is a platform for continuous inspection of code quality.

Create SonarQube User: Adds a user named sonarqube.

Install SonarQube: Downloads and unzips the SonarQube distribution.

Service Configuration: Configures SonarQube to run as a service.

**4. Docker Installation 🐳**
Docker allows you to containerize applications for better scalability and management.

Install Docker: Adds Docker's official repository, installs Docker, and ensures the service is running.

Add Jenkins to Docker Group: Grants Jenkins user access to Docker, enabling it to manage containers.

**🛠️ What this script does:**
User Creation: Automatically creates required users for each application.

Dependency Management: Installs necessary packages like OpenJDK, Docker, and others.

Service Setup: Ensures that Nexus, Jenkins, SonarQube, and Docker are all configured to start on boot using systemd.

Automation: Fully automates the installation and setup process with minimal user interaction.


**📦 Dependencies:**
OpenJDK 17

Docker

Nexus 3.x

Jenkins

SonarQube 10.x


This script simplifies the setup of these essential development tools, ensuring a smoother workflow for your DevOps needs! 🌟

Feel free to modify or expand this further if needed!
