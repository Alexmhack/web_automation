# web_automation
Automating website with bootstrap and node.js

# Objective
Making a website that is automated with user preference using node.js bootstrap and brandflow
from bootstrap tutorial.

# Configuration
install: 
1. Node.js
2. git
3. live-server
4. https://mdbootstrap.com/wp-content/themes/mdbootstrap4/content/jquery/tutorials/brandflow/tutorial-1/2/test-template.zip

Note: To install live-server enter command
npm install -g live-server

Login into BrandFlow account from https://brandflow.net using google authentication

# Checking
Unzip the test template folder and git bash in it. Enter live-server in git bash, you should see 
the welcome page

# BrandFlow
On the /app/containers page click on Create new containers.

Next we have to select our protocol http or https and domain for our website.

Because we have setup our website in local environment we will select http and locahost/ as domain
then click 'save'. To activate our container we need to click on the power button(small button in 
the end).

copy brandflow script from /app/brandflow-script and paste the script in head section between the 
comments.

We have to create a condition based on the button #test-button in brandflow.
In brandflow click on the sidenav and go to automation > conditions. Create new rule and enter the
fields as Condition: Test condition, Type: Click ID, Operator: equals, Param: test-button (id of 
our button), then save the rule.