# simple-php
Simple PHP project to be used for testing openshift


Use the following commands from openshift to deploy



##### Create a new project
`oc new-project simple-project --description="Simple Project" --display-name="A very simple project"`



##### Create a new app. php template is automatically chosen when it sees index.php in the project
`oc new-app https://github.com/satishbabu/simple-php`



##### Create route to expose the app
`oc expose svc/simple-php`



##### Get the URL for the newly crated app
`oc get routes`



##### Check the website
`curl <url from above command>`
