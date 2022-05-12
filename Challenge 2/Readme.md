
Challenge 2
=================
We need to write code that will query the meta data of an instance within aws and provide a json formatted output. 
The choice of language and implementation is up to you.

AWS-Metadata-json
=================

What it does
=================
•	Query the metadata of an ec2 instance within AWS and provide a json formatted output.
•	Retrieve the value of a particular data key.

How to install
=================
•	Create an EC2 Linux instance on AWS
•	SSH into the instance
•	Install Python 3 and git on your instance 
   o	sudo yum install python3 git
•	Clone this repository 
   o	git clone https://github.com/bluprince13/aws-metadata-json
•	Install pipenv 
   o	sudo pip3 install pipenv
•	Open the repository on your instance 
   o	cd aws-metadata-json
•	Install project dependancies 
   o	pipenv install

How to run
===============
•	Open the src folder 
    o	cd aws-metadata-json/src
•	Run whichever script you need: 
    o	python3 get_metadata.py
    o	python3 get_key.py

How it works
================
•	It makes use of the http://169.254.169.254/latest/meta-data link-local address. Instance metatada is provided at this link, 
   but only when you visit it from a running instance.
•	A few simple Python scripts are used to extract the required information using the above API.

