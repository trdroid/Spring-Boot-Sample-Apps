### Creating the project

```sh
$ spring.bat init -dweb, data-jpa, h2, thymeleaf --build gradle GradleAppWithFeaturesAdded
java.lang.IllegalArgumentException: Only the target location may be specified
        at org.springframework.util.Assert.isTrue(Assert.java:68)
        at org.springframework.boot.cli.command.init.InitCommand$InitOptionHandler.createProjectGenerationRequest(InitCommand.java:218)
        at org.springframework.boot.cli.command.init.InitCommand$InitOptionHandler.generateProject(InitCommand.java:209)
        at org.springframework.boot.cli.command.init.InitCommand$InitOptionHandler.run(InitCommand.java:189)
        at org.springframework.boot.cli.command.options.OptionHandler.run(OptionHandler.java:84)
        at org.springframework.boot.cli.command.OptionParsingCommand.run(OptionParsingCommand.java:54)
        at org.springframework.boot.cli.command.CommandRunner.run(CommandRunner.java:219)
        at org.springframework.boot.cli.command.CommandRunner.runAndHandleErrors(CommandRunner.java:171)
        at org.springframework.boot.cli.SpringCli.main(SpringCli.java:54)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
        at java.lang.reflect.Method.invoke(Unknown Source)
        at org.springframework.boot.loader.MainMethodRunner.run(MainMethodRunner.java:48)
        at org.springframework.boot.loader.Launcher.launch(Launcher.java:87)
        at org.springframework.boot.loader.Launcher.launch(Launcher.java:50)
        at org.springframework.boot.loader.JarLauncher.main(JarLauncher.java:58)
        
$ spring.bat init -dweb,data-jpa,h2,thymeleaf --build gradle GradleAppWithFeaturesAdded
Using service at https://start.spring.io
Project extracted to 'C:\Users\droid\onGit\spring-boot-tryouts\_misc\Templates\GradleAppWithFeaturesAdded'
```

The command used above uses the following switches to create a Gradle based Spring Boot web application:

* dweb: to include the library to handle web files that also includes an embedded Tomcat server
* data-jpa: to include a library to handle persistence 
* h2: to include the H2 database engine
* thymeleaf: to include the thymeleaf view engine

### Project Structure and content

![](_misc/Project%20structure%20and%20content.PNG)
