maven-repo
==========

my humble maven repository

for snapshots use:
--
    http://hakandilek.github.com/maven-repo/snapshots/

for releases use:
---
    http://hakandilek.github.com/maven-repo/releases/

with play framework 2.x:
----

    val main = PlayProject(appName, appVersion, appDependencies, mainLang = JAVA).settings(
        resolvers += "release repository" at  "http://hakandilek.github.com/maven-repo/releases/",
        resolvers += "snapshot repository" at "http://hakandilek.github.com/maven-repo/snapshots/"
    )


have fun!
