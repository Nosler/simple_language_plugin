# A Simple Jetbrains Language Plugin

### Authors:
Sam Champer <br/>
Andrea Nosler

### Description

This is a minimal target for an IntelliJ IDEA plugin. This plugin could act as a starting point to implement a more 
complicated grammar, as this project demonstrates the bare necessities that a language plugin requires.
These bare necessities include a grammar, a lexer, associated Java files, and a Gradle file. This plugin includes
syntax hightlighting, custom file extension support, as well as custom icons associated with file types. We have also
made a minor change to the lexer that extends what types of strings are recognized as commends, 
demonstrating how powerful the lexer tool is at customizing a plugin.

This project compiles a plugin that allows for syntax highlighting of "properties" files with a '.simple' filetype.

This plugin is a reimplementation the Jetbrains custom language plugin tutorial located here:
https://www.jetbrains.org/intellij/sdk/docs/tutorials/custom_language_support_tutorial.html,
with a git repositorty here:
https://github.com/JetBrains/intellij-sdk-docs/tree/master/code_samples/simple_language_plugin.

We believe that plugins utilizing the DevKit framework may have portability limitations as compared
to plugins using Gradle, so we reimplemented the simple plugin using the Gradle framework.
This plugin demonstrates the minimal structure of a .gradle file.

### Prerequisites:
1. Java: https://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html
2. Gradle: https://gradle.org/install
3. IntelliJ IDEA: https://www.jetbrains.com/idea/

### Installation:
1. Start IntelliJ IDEA.
2. Choose the "Import project", or select this option from the File menu.
3. Select the build.gradle file in the project folder.
4. Check **"Use auto import"** and **"Create directories for empty content roots automatically"**.
5. Choose your Gradle install location as Gradle home.
6. After loading, open the Gradle tab on the right-hand side of the IDE.
    - At this point you can test the plugin via the **runIde** Gradle task, which will 
    open a new IDE window with the plugin already installed
7. Execute the **buildPlugin** Gradle task.
8. Open **Files** > **Settings** > **Plugins**.
9. Select the gear, then **"Install Plugin from Disk"**.
10. Browse to ``simple_language_plugin/build/libs``, and import ``simple_language_plugin-X.Y.jar``.
11. Restart IntelliJ IDEA.
12. You can now open .simple files and enjoy correct parsing and syntax highlighting of such files in any project
you open with the IDE. To see a sample .simple file, open demo_file.simple in the project root directory.
