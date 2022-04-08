# DilaraBulbulHW1

https://developer.okta.com/blog/2019/09/23/tutorial-build-a-maven-plugin was used to learn the maven plugin concept.

Every file has a unique hash number. The plugin that is build like following helps to resolve the git version number.

1. Firstly, create a maven project(You need to have Java8 and Apache Maven)
2. Add maven dependencies to the pom.xml (Necessary dependencies:maven-core, maven-plugin-api, and maven-plugin-annotations.)
3. You can control last versions and take dependencies from-->https://mvnrepository.com/
4. Then you need to build plugins,plugin
5. Each maven project has a goal and this goal is defined thanks to @Mojo 
6. After handled all these mentioned above, then it is time to build project with:
  
  ```
  mvn install 
  ```
7. If all dependendencies and plugin versions are Ok, you need to see "BUILD SUCCESS" as an output
8. We need to write the execute command to see the the version number
9. Important step is adding reporting codes to the pom.xml
10. Then it is time to run project with:
 
  ```
mvn com.okta.example:example-maven-plugin:version
  ```
11. Program output will be like following;
![image](https://user-images.githubusercontent.com/97522259/162533204-811db53a-7f6e-4e09-90a6-80ceeac62dcd.png)
