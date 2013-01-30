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
        resolvers += Resolver.url("release repository", url("http://hakandilek.github.com/maven-repo/releases/"))(Resolver.ivyStylePatterns),
        resolvers += Resolver.url("snapshot repository", url("http://hakandilek.github.com/maven-repo/snapshots/"))(Resolver.ivyStylePatterns)
    )


have fun!
