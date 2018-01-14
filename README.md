# Certifier Project

[![Gitter chat](https://badges.gitter.im/gitterHQ/services.svg)](https://gitter.im/jboss-outreach)

## Contents
* [What is Certifier?](#desc)
* [Setting up](#setup)
* [Running the App](#run)
* [Contributing](#contribute)
* [Additional Learning](#learning)

## <a id="desc"></a> What is Certifier?
This project generates a certificate. It runs on Vert.x, and is built on the Gradle build system.

#### Features
* Students can generate certificates of completion for a variety of courses.
* Mentors can generate bulk certificates for students from data in CSV files.

## <a id="setup"></a> Setting Up the Project

**If you want to just download the app**

- Just download [zip](https://github.com/jboss-outreach/certifier/archive/master.zip) file.

**If you want to contribute to the project**

1. **Fork** the repository by clicking on the Fork icon at the top right corner of this page.
2. **Clone** the repository on to your local machine by running the following commands on git:
```
$ git clone https://github.com/[YOUR-USERNAME]/certifier.git
```

3. If you need help, refer [Forking and Cloning in git](https://help.github.com/articles/fork-a-repo/). You can also ask for help on the [chat](https://gitter.im/jboss-outreach/gci).

#### Setup Dependencies
* [Java JDK 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) (Don't use Java 9 as it won't work)
* [Gradle 4.0.0](https://gradle.org/releases/) or higher

## <a id="run"></a> Running the app

### Set up in your local machine

1. Download [Download JDK 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) (JDK 8, as 9 won't work). Make sure it is for your specific operating system!
2. Make sure you have declared the `JAVA_HOME` environment variable to the directory where JDK was installed.
3. The project can be run by two methods:
	* [Using An IDE like Intellij IDea or Eclipse that supports Java Development](#ide)
	* [Via Command User Interface](#cui)

#### <a id = "ide"> </a> Using an IDE

##### Using IntelliJ Idea
1. Download and install [Intellij Idea] (https://www.jetbrains.com/idea)
2. Configure Intellij project defaults, project structure, to set the project SDK to java version 1.8:

    ```
    configure --> Project Defaults --> Project Structure --> Select JDK 1.8 location
    ```

	* [Refer this for further help](https://www.jetbrains.com/help/idea/defining-a-jdk-and-a-mobile-sdk-in-intellij-idea.html)
3. Import the cloned repository into your IDE
4. After importing there should be a notification in the bottom right, asking you to link the project to gradle. Click on it and it will occur automatically.
5. Right click the **App** class
6. Right click on the vertx at the top of the code and use the suggested help from intelliJ to link it to the project
7. Click **Run App.main()**

##### Using Eclipse IDE
1. Download and install [Eclipse IDE](https://eclipse.org/)
2. Get gradle plugin for Eclipse from [here](https://steffenschaefer.github.io/gwt-gradle-plugin/doc/latest/eclipse)
3. Configure Eclipse project defaults, project structure, to set the project SDK to java version 1.8:

	```
    Window --> Preferences --> Java --> Compiler --> Set Compiler Compliance Level to 1.8
    ```
4. Import the cloned repository into your IDE.
5. Implement vert.x in the project.
5. Click **Run App.main()**

#### <a id = "cui"> </a> Running via the Command User Interface

##### If using on terminal in Linux/Unix,
```sh
$ ./gradlew run # pwd should be project home dir
```
* If permission is denied then use `chmod +x ./gradlew`

##### If using on Command Prompt in Windows
```sh
$ gradlew run   # pwd should be project home dir & open cmd as admin
```

### Viewing the App
* Open http://localhost:4000 in your browser

## <a id="contribute"></a> Contributing to the project

**Step 1: Fork this project:**

Go to the top right of the project page and click on "Fork". A fork of this repo will be created on your GitHub account.

<a id="step2"></a> **Step 2: Code your changes**:

Create a new branch by:
```
$ git checkout -b YOUR_NEW_BRANCH_NAME
```
Then create/edit files as per your coding requirements. Ensure that your code is clean and efficient, and avoid redundancies. It is also advised to follow naming conventions as and where specified. Also make sure that your code is your own, and is not closed-source or stolen.

We use branches because they are very useful when you have multiple Pull Requests in the same repository.

**Step 3: Commiting and pushing the changes:**

*Commit* the changes and *push* the commit to your forked repository on GitHub by:
```sh
$ git add path/to/your/file    # for including inidividual files.
$ git add .     # for including all files at once
```
```sh
$ git commit -m "DESCRIBE YOUR CHANGES"
$ git push origin
```
If stuck at this point, refer [here](https://readwrite.com/2013/10/02/github-for-beginners-part-2/)

**Step 4: Creating a Pull Request:**

Once you are done coding the changes, commit the files and create a [*Pull Request*](https://help.github.com/articles/about-pull-requests/). Click on "Compare across forks" when creating the Pull Request, and select the master branch of this repo as the base. Set the head to your branch that your committed onto. Click on the button _Create Pull Request_. Give your Pull Request a meaningful title and a brief message explaining the purpose of your commits.

**Step 5: Ensuring code quality**

Once a Pull Request has been created, check if it can be merged without any conflicts. If there are any issues, repeat the process starting [***Step 2***](#step2) and try to resolve them. Wait for a reviewer to cross check your changes. If your work is satisfactory, the reviewer will merge your changes. They may also request additional changes, which you should implement and, then update the Pull Request.

* Additional Reference regarding cloning, forking and editing a repository are available [**here**](https://egghead.io/lessons/javascript-how-to-fork-and-clone-a-github-repository).


`Keep Contributing to open source!` :smile:


## <a id = "learning"> </a> Additional Learning

- [Git Handbook](https://guides.github.com/introduction/git-handbook)
- [Git Introduction](https://guides.github.com/introduction/flow)
- [Terminal Handbook](http://linuxcommand.org/)
- [Command Prompt Handbook](http://www.makeuseof.com/tag/a-beginners-guide-to-the-windows-command-line/)


Happy Coding!
