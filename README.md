# droidquest
DroidQuest, both the Android version and the normal Java version.

See https://github.com/ThomasFooteDQ/DroidQuest for the code that I branched from.

The above repository contains only a Java version of the game. I modified that code extensively to split it into 3 separate modules. One is the shared Java code that can be compiled as either an Android library or a plain java library. Another is the Android specific code. The last is the Java specific code.

The problem originally was that Android obviously does not support pure Java. As such, it was necessary to refactor things extensively, but I wanted to have the ability to fix bugs in both versions at the same time. This is a little weird, but on my machine the shared library directory is referred to by two different IntelliJ projects (the Java app version and the Android version).
