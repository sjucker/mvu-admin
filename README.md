# MVU Admin

## Deploying to Heroku
### Choose a JDK
* Make sure there is a `system.properties` file defining the wanted Java runtime
  * `java.runtime.version`
### Customize Maven
* `MAVEN_CUSTOM_GOALS`: `clean dependency:list package -Pproduction`
* Add this to Settings -> Config Vars in Heroku Dashboard

### CLI Commands
* Cancel current build:
  * `heroku builds:cancel -a mvu-admin`
