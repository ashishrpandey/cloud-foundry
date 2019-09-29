Step 1. Check the app list:

To start, we should see what is currently running for us.

    $ cf apps

Step 2. Clean up the Web App:

The Web app needs to be removed and you can remove the created route with the -r option:

    $ cf delete web-app -r -f

Step 3. Clean up the Worker App:

    $ cf delete worker-app -f

Step 4. Check the app list again:

    $ cf apps
