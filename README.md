Here's how to safely edit the /etc/sudoers file:
Open the /etc/sudoers File Safely: Use the visudo command, which ensures syntax checking and more safety than directly editing the file.Run:

sudo visudo

Add the Passwordless Sudo Entry: In the editor that opens, add the following line to grant server3 passwordless sudo privileges:

"user" ALL=(ALL) NOPASSWD: ALL          #till exp: server3 ALL=(ALL) NOPASSWD: ALL

