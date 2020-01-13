# DeploySinatraApp
 Deploy a sinatra application using cloudformation

# How to use this

Download this project, upload "DeploySinatraApp.json" to AWS Cloudforamtion to create a stack. After the stack is created, the sinatra app will run on port 80

# Note

1.Make sure you have a valid Amazon EC2 key pair and record the key pair name before you create the stack.
To see your key pairs, open the Amazon EC2 console, then click Key Pairs in the navigation pane.
If you don't have an Amazon EC2 key pair, you must create the key pair in the same region where you are creating the stack.

2.You must not changed the user name for AMI, as the app will be installed under ec2-user.

# Why I choose CloudFormation

1.It is simple. 
AWS CloudFormation enables user to model entir infrastructure inside a document. This helps user to standardize infrastructure parts used across the user organization and quicker troubleshooting

2.Everything is automated.
AWS CloudFormation proviions resources in a safe manner. Users do not need to perform manual actions or write custom scripts in a repeatable manner. CloudFormation also roll back changes automatically if errors are detected.

3.It is easy to manage. 
Its configuration-as-code feature enable users to check in templates into version control system,modify in any code editor, and collaborate with team members before delopying into production.

# Future Improvements

1.Introduce AWS Auto Scaling Groups and load balancer

2.Implement this in Ansible as ansible is more flexible. It supports more cloud platforms while CloudFormation is only for AWS. 

3.Introduce Docker as it is more cost-effective and more efficient with regards to CI and configurations.


