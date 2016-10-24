# AWS
To run the above code follow the below points in ubuntu 14.0.4 version:
i) Install the python ansible by using the command "sudo apt-get install ansible"
ii) Download the above repository 
iii) Assign the values in vars/main.yml for the variables given in playbook.yml
example:
---

aws_access_id=[********]

aws_secret_id=[********]

region=[*******]

test=[***.pem]

Once you run the code by giving these variable it will launch the ebs with simple web application as i deployed.
It will automatically scale up and scale down through network input.If the network traffic is more than 20,00,000 
it will autmatically launch a new instance and if it is less then it will automatically delete the instance
