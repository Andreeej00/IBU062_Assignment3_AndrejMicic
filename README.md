# IBU062_Assignment3_AndrejMicic
#Task 1
In this task, you will create a simple computer network using Packet Tracer. The network should look like this:
Add a router and two switches to the network, and connect the switches to the router.
Connect two PCS, one laptop and one server to the first switch.
Connect two servers and one PC to the second switch.
Set up DHCP on the router so that all connected hosts (PCs, laptops and servers) get IP addresses automatically. Use the following information:
For the hosts connected to first switch:
Network address: 168.90.0.0 
Router address (default gateway): 168.90.0.1
Subnet mask: 255.255.0.0
For the hosts connected to the second switch:
Network address: 210.3.14.0 
Router address (default gateway): 210.3.14.1
Subnet mask: 255.255.255.0
Use the “Note” tool in Packet Tracer, and denote the IP address that each host has received next to the device.
Test the connectivity between the laptop device connected to the first switch to one of the servers on the second switch using the “ping” tool and take a screenshot of the interaction.
Test the interaction in both directions: from laptop to server, and from laptop to the server.


Task 2
In this task, you will set up version control for the computer network from Task 1. 
Document and collect all your network files.
Create a new empty folder where you will keep all assignment data.
In this folder, create a new file named network-setup.md.
In the network-setup.md file, you should:
List all the devices that appear in your network, along with a model of the device (if applicable; namely for routers and switches).
Next to each host, note down what IP address was assigned to it.
Copy your Packet Tracer file (.pkt) to the folder.
Create a new folder called screenshots, where you will add the two screenshots of using the “ping” tool from Task 1.
Commit and push your work to a Git repository.
Initialize a Git repository in the folder you created.
Stage and commit all the files with the message “Initial submission of Packet Tracer network.”
Create a remote repository on GitHub named like this:
 “IBU062_Assignment3_NameSurname” 
   (e.g. IBU062_Assignment3_AldinKovacevic)
Connect your local repository to the remote repository you created.
Push your changes to your GitHub repository.
Make an update to your repository.
After the initial commit and push, update your Packet Tracer file to add one more PC to each switch (and make them use DHCP).
Update the network-setup.md file to include the information about two new PCs.
Stage and commit your changes with the message: “Added new PCs to the configuration.”
Push your changes to your GitHub repository.
Create a new branch.
Create a branch named add-dhcp-details.
Switch to this branch, and update network-setup.md to explain the exact DHCP commands and steps  you used on the router to set up DHCP.
Stage and commit your changes with the message: “Added DHCP configuration details.”
Push the new branch to your GitHub repository.
Create a pull request (PR).
On GitHub, create a pull request (PR) from the add-dhcp-details branch.
Write a short PR description explaining the changes.
Merge the PR changes to the master / main branch.
Tag the latest version.
Pull the merged changes to your local repository.
Create a tag named v0.1 from the latest master (including the DHCP document updates).
Push the tag to your GitHub repository.


Assignment Submission Details
For this assignment, you will need to submit your GitHub repository link on LMS. At the end of the assignment, your repository should contain both Task 1 and Task 2. Make sure that your GitHub repository is public. If we cannot access your repository after the deadline, you will get no points.
Important note: You should use Git tools and commands for (most of) Task 2. Do not use the “upload files / create new file” feature from GitHub - you will get no points from Task 2 if you do so.

The deadline for submission is December 17th, 2024, 23:59. 
