PHP App Engine patch for DrEdit
===============================

A patch for the [DrEdit (Google Drive Editor) PHP](https://github.com/googledrive/dredit/tree/master/php) example that will allow it to run on [Google App Engine](http://cloud.google.com/appengine)

## Setup Instructions

1. Clone the DrEdit repository:

  `git clone https://github.com/googledrive/dredit.git`

1. Ccopy the contents of the php directory into your working directory.

1. Download a copy of the app.yaml file found in this repository.

1. The first line will look like this:

  `application: replace-with-your-app-id`

  Edit the __app.yaml__ file, replacing the string __replace-with-your-app-id__ with the ID of your App Engine app.

  For example, if my App Engine app id was __app1234__ then the line would look like this after editing:

  `application: app1234`

1. Follow steps 3 to 8, and 10 from the original PHP instructions https://github.com/googledrive/dredit/blob/master/php/README.md

1. Finally upload/update your App Engine app, by running:

  `appcfg.py update .`
