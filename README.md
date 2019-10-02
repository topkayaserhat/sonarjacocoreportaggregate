# README #


### Requirements ###

* Java 7+
* Maven 3.2+

### Building and running from command line ###

```
mvn clean verify
```


# Data files (.exec) take place under : target/coverage-reports

# Jacoco test files take place under : target/site/

# If you would like to send the coverage report the sonar :

mvn sonar:sonar \
 -Dsonar.projectKey=test \
 -Dsonar.host.url=http://34.254.243.134:9000 \
 -Dsonar.login=186fb0ac85b4497346f69c49079c30ed7fd65c53 \
 -Dsonar.jacoco.reportPath=target/coverage-reports/aggregate.exec \
 -Dsonar.junit.reportPaths=target/surefire-reports,target/failsafe-reports \

