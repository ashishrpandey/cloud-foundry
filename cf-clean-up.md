Step 1. Check the app list:

To start, we should see what is currently running for us.

    $ cf apps

Step 2. Clean up the Web App:
Only "cf delete app-name" command will stop the application, destroy the containers, and remove the applications blobs. 
This command does not remove any routes that were created. 

You can remove the web-app along with the created route with the -r option:

    $ cf delete web-app -r -f

Step 3. Clean up the Worker App:

    $ cf delete worker-app -f

Step 4. Check the app list again:

    $ cf apps
