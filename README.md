Project Overview:

The assignment involves creating an automated deployment solution for customer environments to streamline the process of transitioning to dedicated hardware and facilitating their conversion into paying customers. This documentation provides a detailed explanation of the objectives, steps, and components involved in the deployment process.

Objectives:

1-Develop an automated configuration process for customer deployments.

2-Simplify the deployment procedure to enhance customer experience.

3-Enable smooth migration to dedicated hardware for customers.

4-Facilitate the monetization of customer deployments.

Components:

1-Automation Script: Utilize Ansible to create scripts that automate the deployment process.

2-Customer Portals: Develop open-source portals similar to Hub.itsl for customer interaction and access to services.

3-Email Notifications: Configure automated email notifications to inform customers about their deployed environments.


Project Structure
Ansible project directory is structured as follows:

/ansible-project
    /roles
        
        /software_installation
            /tasks
                main.yml
        
        /web_server_configuration
            /tasks
                main.yml
        
        /email_notification
            /tasks
                main.yml


1-/software_installation: This directory holds tasks related to software installation. It's structured in a way that separates concerns, making it clear that tasks within this directory are specifically related to installing software components.

2-/web_server_configuration: Here, tasks for configuring the web server are stored. This directory is dedicated to tasks related to setting up and configuring the web server. Again, it's a clear separation of concerns, which is good practice for maintaining an organized project.


3-/email_notification: This directory contains tasks for managing email notifications. It's structured similarly to the other directories, with a clear focus on tasks related to email notifications.


4-main.yml files: Each directory has a main.yml file, which is likely used to define and organize tasks. This is a common convention in Ansible projects, where the main.yml file serves as an entry point for the tasks within that directory.


Here's how to safely edit the /etc/sudoers file:
Open the /etc/sudoers File Safely: Use the visudo command, which ensures syntax checking and more safety than directly editing the file.Run:

sudo visudo              #till exp: server3@ubuntuserver3:~/customer$ sudo visudo

Add the Passwordless Sudo Entry: In the editor that opens, add the following line to grant server3 passwordless sudo privileges:

"user" ALL=(ALL) NOPASSWD: ALL          #till exp: server3 ALL=(ALL) NOPASSWD: ALL

