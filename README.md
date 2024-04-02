Assignment 4

Network Automation with AWX Tower

Chance Page

TELE36058

Professor Sebastian Maniak

February 29, 2024

**Part 1: Installation of Ansible AWX**

I started my journey by installing Ansible AWX on a Ubuntu VM. The first step was to deploy a Ubuntu VM, which was a straightforward process. Once the VM was up and running, I cloned the Ansible AWX GitHub repository and navigated to the installer directory.

Running the installation playbook using Ansible was an interesting experience. It was fascinating to see how Ansible automated the deployment of AWX. After the installation was complete, I verified it by accessing the AWX web interface. The interface was user-friendly and intuitive, making it easy to navigate and understand.



Figure 1: Web GUI

**Part 2: Configuring Ansible AWX**

The next step was to configure AWX to manage network devices. This involved setting up inventories, credentials, and projects. I created an inventory named NetworkDevices and manually added a couple of mock network devices to it.

Setting up SSH credentials in AWX was a breeze. These credentials would be used for accessing the mock network devices. I then linked a new project in AWX to a GitHub repository. This repository contained Ansible playbooks for network automation, which would be crucial for the next part of the assignment. ![A screenshot of a computer


Figure 2: Credentials



Figure 3: Inventory


Figure 4: Project:

**Part 3: Creating and Running Ansible Jobs**

With the setup complete, it was time to create and run Ansible jobs for network device configuration. I created a job template in AWX using the previously created project, inventory, and credentials.

Figure 5: Job

Executing the job template was as simple as clicking a button. I monitored its execution in the AWX dashboard, which provided real-time updates and logs. I also created a workflow that deploys 2-3 different jobs and a survey within a job that allows users to input data. The survey included a list, checkbox, and input text.



Figure 6: Job Output


Figure 7: Survey



Figure 8: Workflow

**Part 4: Reflection and Exploration**

In the final part of this assignment, I delved deeper into the features of AWX and reflected on my learning experience. I explored various features such as scheduling jobs, setting up notifications, and using dynamic inventories.

One particular feature that stood out to me was the ability to set up custom notifications. For instance, I found that I could create a notification named “Interface Overwritten”. This notification would ping a Slack channel every time an interface is overwritten. This feature is incredibly useful as it allows for real-time updates and immediate action when necessary.


Figure 9: Notifications

Reflecting on the potential of AWX and Ansible for automating tasks beyond network configuration, I realized the immense possibilities that these tools offer. They can significantly reduce manual effort and increase efficiency in various IT domains. The power of automation is truly transformative, and tools like AWX and Ansible are leading the way.

Evaluation

In terms of the evaluation criteria, I believe I have successfully completed the assignment. The installation and configuration tasks were completed accurately, and I was able to create and execute Ansible jobs within AWX. The reflective essays and reports provide a deep understanding of the concepts, and I explored additional AWX features creatively, with a special focus on the custom notifications feature.
