
Copyright (C) 2014 Google Inc.

# Sample 'hello world' application for use with the App Engine Java VM Runtime.

Requires [Apache Maven](http://maven.apache.org) 3.1 or greater, and
JDK 7 in order to run.  This application needs to be deployed to the
[App Engine VM Runtime][1].

Make sure that you are invited to the [VM Runtime Trusted Tester
Program][2], and have [downloaded the SDK](http://commondatastorage.googleapis.com/gae-vm-runtime-tt/vmruntime_sdks.html).

To build, do the following:

1. Change the value of the `application` element in your `appengine-web.xml` to the app
id of an app that has been whitelisted for the VM Runtime.
2. Run `mvn package`
3. Run the `appcfg.sh` script from the VM Runtime SDK as follows:

        $ $SDK_DIR/bin/appcfg.sh -s preview.appengine.google.com update target/hello-1.0-SNAPSHOT

4. Visit `http://your-app-id.appspot.com/`.

For further information, consult the [Java App
Engine](https://developers.google.com/appengine/docs/java/overview)
documentation.

To see all the available goals for the App Engine plugin, run

    mvn help:describe -Dplugin=appengine

[1]: https://docs.google.com/document/d/1VH1oVarfKILAF_TfvETtPPE3TFzIuWqsa22PtkRkgJ4
[2]: https://groups.google.com/forum/?fromgroups#!topic/google-appengine/gRZNqlQPKys
[3]: https://cloud.google.com/console
