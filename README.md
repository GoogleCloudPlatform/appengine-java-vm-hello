
Copyright (C) 2014 Google Inc.

# Sample 'hello world' application for use with the App Engine Java Managed VMs.

Requires [Apache Maven](http://maven.apache.org) 3.1 or greater, and
JDK 7 in order to run.  This application needs to be deployed to the
[App Engine VM Runtime][1].

Install the [Cloud SDK for Managed VMs](https://cloud.google.com/appengine/docs/managed-vms/)
To run the application, do the following:

1. Set the correct Cloud SDK project via `gcloud config set project YOUR_PROJECT`
id of your application.
2. Run `mvn gcloud:run`
4. Visit http://localhost:8080
5. To deploy, run `mvn gcloud:deploy`
6. Visit `http://YOUR_PROJECT.appspot.com`.
