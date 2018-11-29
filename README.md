Demonstrates a issue in maven-publish plugin in Gradle 4.10.2

To reproduce: run `gradle clean cleanRepo publishToMavenLocal build`

The above will fail.

Goto -> myLib -> build.gradle -> comment out line `classifier = "jdk18"` and run the same command again.
Build will succeed
