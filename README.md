# hadoop_project
initially i created an linux instance on aws account using ec2 service.
then i configured that instance to connect locally by password.
to do so click on connect.
check mark third option and it opens terminal.
type echo lnbdevops077 |passwd ec2-us --stdin to change password.
goto vim /etc/ssh/sshd_config and go to line number and do passwordauthentication to yes 
then do systemctl restart sshd
then go to your local ubuntu terminslk and type ssh ec2-user@ip then passwoed lnbdevops077.
you are inside the instance locally 
yum install httpd python3 -y
systemctl start httpd 
systemctl enable httpd
open ms vscode and open folder on desktop names devops_project
inside that project cresagte padwe index.html
create form and copy that code to the /var/www/html
before it remove the default index.html by rm index,html
then again create by vim index.html and paste the copied code here 
now whenever you access the intance ip from anywhere it will show the contgents of this index.html.
now when you enter the submit button this should take you to the another page clalled check.py which checks the username and password and on authentication print successfully llgged in.
to check username and password there are two methods 
one is to cfreate a seperagter database server and authenticate from there or use python dictionary.which stores data in kdey valu pair and use python-cgi(common gaTEWAY INTERFACE),flask,django.









