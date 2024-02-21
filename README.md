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





Here's how to safely edit the /etc/sudoers file:
Open the /etc/sudoers File Safely: Use the visudo command, which ensures syntax checking and more safety than directly editing the file.Run:

sudo visudo              #till exp: server3@ubuntuserver3:~/customer$ sudo visudo

Add the Passwordless Sudo Entry: In the editor that opens, add the following line to grant server3 passwordless sudo privileges:

"user" ALL=(ALL) NOPASSWD: ALL          #till exp: server3 ALL=(ALL) NOPASSWD: ALL

