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

# Brandflow condition
We have to create a condition based on the button #test-button in brandflow.
In brandflow click on the sidenav and go to automation > conditions. Create new rule and enter the
fields as Condition: Test condition, Type: Click ID, Operator: equals, Param: test-button (id of 
our button), then save the rule.

# Brandflow wrapper
We have a condition, now we can create a wrapper around it. Goto sidenav > Dynamic content > Lists
Then click on create new wrapper, enter the name for wrapper, we will create a welcome card when 
the user clicks on the button, so name the wrapper Welcome card, for the code paste the code from 
the tutorial in the code section and you can see the preview for our card.

# Setting the trigger
Wrapper and condition have been set but we have no trigger for our dynamic content to show up.
To set our trigger, inside the content section click on the add button and in the section for 
triggers for our wrapper click on add button and name our trigger Welcome card trigger, click
on Condition and from the options select the button test-button and click on set and save the 
trigger.

# Publishing Changes
After we have set the condition, wrapper and the trigger for our condition we have to click on 
the button at top saying publish changes, publish the changes.

# Checking
run the live-server using the command live-server and click on the button, the welcome card will
appear on the right where our test-wrapper is set

# Actual Project work
All above was seeing how brandflow works, now we will work on our real project. Open the 
index.html file from CreativeFolks.zip and paste our brandflow script in head tag.

NOTE: live-server serves the html file with name index on localhost port 8080