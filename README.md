PHP App Engine patch for DrEdit
===============================

A patch for the [DrEdit (Google Drive Editor) PHP](https://github.com/googledrive/dredit/tree/master/php) example that will allow it to run on [Google App Engine](http://cloud.google.com/appengine)

https://github.com/googledrive/dredit/tree/master/php

Download a copy of the app.yaml file found in this repository.

The first line will look like this:

    application: replace-with-your-app-id

Edit the __app.yaml__ file, replacing the string __replace-with-your-app-id__ with the ID of your App Engine app.

For example, if my App Engine app id was __app1234__ then the line would look like this after editing:

    application: app1234

Now upload/update your App Engine app, by running:

    appcfg.py update .
