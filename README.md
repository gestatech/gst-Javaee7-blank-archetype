# JavaEE 7: Blank Archetype
A totally blank configuration ready JavaEE 7 Project.

What does it contain:
- Empty Java EE Project structure - maven build and deploy ready
- Example beans.xml for CDI
- Example perstistence.xml for JPA
- Example JAXRSConfig.java for JAX-RS Web Services

All configuration files have the extension .example by default, so they are not directly active.
If you want to use CDI for example just remove the .example extension and your ready to go.
Need a database remove .example extension from persistence.xml, same for JAX-RS,...

How to use with interactive mode:
```sh
mvn archetype:generate -Dfilter=be.gestatech:gst-javaee7-blank-archetype
```

How to use with non interactive mode:
```sh
mvn archetype:generate                        \
-DarchetypeGroupId=be.gestatech                  \
-DarchetypeArtifactId=gst-javaee7-blank-archetype \
-DarchetypeVersion=1.0.0-SNAPSHOT                        \
-DgroupId=<yourGroupId>                       \
-DartifactId=<yourArtifactId>                 \
-Dversion=1.0.0-SNAPSHOT
```

Remove ```.example``` extension on sample configuration files as needed.