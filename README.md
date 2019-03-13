# CIS407: IDE Extension Plugins

We implemented the Jetbrains custom language plugin tutorial. There may be portability issues with DevKit, so we utilized Gradle instead. It compiles a plugin that allows for syntax highlighting of "properties" files with the .simple filetype.

### Authors:
Sam Champer <br/>
Andrea Nosler

### Prerequisites:
1. Java: https://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html
2. Gradle: https://gradle.org/install
3. IntelliJ IDEA: https://www.jetbrains.com/idea/


### Installation:
1. Start IntelliJ IDEA
2. Import the project
3. Select the build.gradle file in the project folder
4. Check **"Use auto import"** and **"Create directories for empty content roots automatically"**
5. Choose the Gradle install location as Gradle home
6. After loading, open the Gradle tab on the right-hand side
7. Execute the **runIde** Gradle task
