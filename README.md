# HockeyAppTest

Facilitates testing of Jenkins [HockeyApp Plugin](https://github.com/jenkinsci/hockeyapp-plugin) changes.

1. Make your changes.
2. Use the Maven goal hpi:run to load a version of Jenkins preloaded with the updates plugin to localhost:8080/jenkins
3. Setup a pipeline or freestyle job and test your changes.
