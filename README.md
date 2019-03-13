# CIS407: IDE Extension Plugins

This is a minimal target for an IntelliJ IDEA plugin. This should act as a starting point to implement a more complicated grammar, as this project demonstrates the bare necessities that a language plugin requires. The bare necessities include a grammar, a lexer, associated Java files, and a Gradle file. 

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
    - At this point you can test the plugin via the **runIde** Gradle task, which will open a new IDE window with the plugin already installed
7. Execute the **buildPlugin** Gradle task
8. Open **Files** > **Settings** > **Plugins**
9. Select the gear, then **"Install Plugin from Disk"**
10. Browse to ``simple_language_plugin/build/libs``, and import ``simple_language_plugin-X.Y.jar``
11. Restart IntelliJ IDEA
