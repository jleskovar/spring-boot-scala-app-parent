# spring-boot-scala-app-parent
Convenient parent pom that can be used for Scala-based Spring Boot applications.

# Usage

Add to the top of your pom:

    <parent>
        <groupId>com.github.jleskovar</groupId>
        <artifactId>spring-boot-scala-app-parent</artifactId>
        <version>1.0.4</version>
    </parent>

# Info

The spring-boot-scala-app-parent sets up the following default maven dependencies:

* Scala 2.11.6 dependency
* [ScalaTest](http://www.scalatest.org/) 2.2.4 test dependency
* [Spring-Boot](http://projects.spring.io/spring-boot/) 1.2.3.RELEASE starter dependency
* [Spring-Boot](http://projects.spring.io/spring-boot/) 1.2.3.RELEASE test dependency
* [Spring Cloud](http://projects.spring.io/spring-cloud/) 1.0.1.RELEASE declared dependency

As well as the following default plugins:

* spring-boot-maven-plugin - to create a fat executable jar
* directory-maven-plugin - creates a ${rootdir} property that is correctly set and referencable from any module in the build
* scalastyle-maven-plugin - runs ScalaStyle against src/main/scala, using config found in ${rootdir}/project/scalastyle_config.xml
* scalatest-maven-plugin - runs tests written using ScalaTest
* maven-surefire-plugin - needed to run regular tests, and to correctly honour skipTests flag


