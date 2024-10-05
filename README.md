# Hello World with Struts2 using Maven

This project is a basic example of a dynamic web application "Hello World! through the Struts2 action". The project was created using the Eclipse for EE IDE and Maven.

## Project structure

![Directories structure of the project](https://github.com/MavapeGZ/HelloWorld-struts2/blob/main/HelloWorld-struts2.jpg)

## Prerequisites

Before executing the project you should have downloaded and installed the following elements:

- [Java JDK](https://www.oracle.com/java/technologies/javase-downloads.html)
- [Apache Maven](https://maven.apache.org/install.html)
- [Eclipse IDE](https://www.eclipse.org/downloads/) (you can use other IDEs, but the configuration may be different)

Note that some versions of the above tools may be incompatible with each other, so make sure to install versions that are compatible with each other.

## Installing and running

Follow the next steps to clone and execute the project.

#### 1. Clone the repository
For this step you need to have installed the [Git](https://git-scm.com/) tool.

Now you need to initialize your local repo, so open a bash in the folder you are going to store the project and type the following commands:

`git init` (Initializes the repo)

`git clone https://github.com/MavapeGZ/HelloWorld-struts2.git` (Clones the repo)

#### 2. Move to the directory

If you are not yet in the directory where you cloned the repo, move there:

`cd HelloWorld-struts2`

#### 3. Compile and clean the project using Maven
We need to compile the project in order to be able to run it later. 

`mvn clean install`

If some errors are appearing in your bash, check the error and fix it. 

##### 4. Run the application with Jetty server

`mvn jetty:run`

If you followed the steps and no errors showed on the screen, congratulations, you did it!

#### 5. Access the website
Now, you should open your favourite browser and tipe the following URL:

`http://localhost:8080/HelloWorld-struts2/`

This is a connection on to your own machine in the 8080 port (the default one). If some error is on the screen, maybe you have this port not available.

## Description of the project
#### Struts2 Action
The [HelloWorldAction.java](https://github.com/MavapeGZ/HelloWorld-struts2/blob/main/src/main/java/org/apache/struts/helloworld/action/HelloWorldAction.java) class handles the HTTP request and delegates the response to the view (JSP).

#### JSP
The [HelloWorld.jsp](https://github.com/MavapeGZ/HelloWorld-struts2/blob/main/src/main/webapp/HelloWorld.jsp) file shows the stored message in the [MessageStore](https://github.com/MavapeGZ/HelloWorld-struts2/blob/main/src/main/java/org/apache/struts/helloworld/model/MessageStore.java) class.

#### Configuration
- [struts.xml](https://github.com/MavapeGZ/HelloWorld-struts2/blob/main/src/main/resources/struts.xml) contains the Struts2 configuration for actions and views.
- [web.xml](https://github.com/MavapeGZ/HelloWorld-struts2/blob/main/src/main/webapp/WEB-INF/web.xml) contains the configuration of the servlet for Struts2 in the deployment descriptor.

## Author

[MavapeGZ](https://github.com/MavapeGZ)

## License
*This project is under MIT License. Check the [LICENSE](./LICENSE) file for more details.*

