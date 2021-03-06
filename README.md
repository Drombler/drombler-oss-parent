# Drombler OSS - Parent POM
This Drombler OSS Parent POM should be the parent (either directly or indirectly) of every Drombler project unless there
 is a good reason to do otherwise (in which case the reason should be documented).
 
| Major Version | Comments |
| ------------- | ------- |
| v4 | <ul><li>Java SE 11</li></ul> |
 
## Build the project from sources
```bash
mvn clean install
```
Please note that the develop branch (SNAPSHOT version) of the project might depend on SNAPSHOT versions of other projects.

If you don't want to build the dependent projects as well, please make sure to define a proxy in your [Maven Repository Manager](https://maven.apache.org/repository-management.html) to the following Maven Repository: https://oss.sonatype.org/content/repositories/snapshots/ and include it in your [single group](https://help.sonatype.com/repomanager3/formats/maven-repositories#MavenRepositories-ConfiguringApacheMaven).
