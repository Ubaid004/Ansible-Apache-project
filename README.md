# Ansible-Apache-project
Write ansible playbook for below tasks:

1. Install apache server and deploy sample html application 2. Create /var/www/example.com

3. deploy a sample application to the above directory 4. create a virtual host for deploy application and set it as default virtualhost.

4. IN THIS PLAYBOOKS, the tasks are as follows:

1 Install Apache web server using the apt module.

2 Deploy the sample HTML application by copying the index.html file to /var/www/example.com/. 3 Create the /var/www/example.com directory using the file module.

4 Set ownership and permissions for the

/var/www/example.com directory using the file module. 5 Create the Apache virtual host configuration file for example.com using the template module. You'll need to provide a template file (virtual_host_template.j2) that includes the necessary configurations for the virtual host.

6 Enable the required Apache modules (rewrite and vhost_alias) using the apache2_module module. 7 Enable the example.com virtual host using the apache2_vhost module.

8 Disable the default Apache virtual host using the apache2_vhost module.
9 Restart the Apache service to apply the changes using the service module.

Remember to replace

/path/to/sample_application/index.html with the actual path to your sample HTML application file, and /path/to/virtual_host_template.j2 with the actual path to your

virtual host template file. Also, ensure that the web servers group in your Ansible inventory file contains the appropriate hosts where you want to install and configure Apache.
