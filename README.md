# UPDATE:

This repo was migrated from the swt-repo project on Google Code. It is moving to [http://maven-eclipse.github.io](http://github.com/maven-eclipse/maven-eclipse.github.io) which provides a reproducible repository and cleaner urls. Currentently it contains SWT from 4.2+, including the 4.4.2, 4.5, and interm RC milestones. JFace and SWTBot jars and dependencies will be added soon.

------------------

A Maven repository hosting SWT and JFace jar files / artefacts which [still](https://bugs.eclipse.org/bugs/show_bug.cgi?id=199302) can't be found in maven central.

### SWT example

Add this repository to your project's pom.xml:

```
<repositories>
    <repository>
        <id>swt-repo</id>
        <url>https://raw.githubusercontent.com/maven-eclipse/swt-repo/master/</url>
    </repository>
</repositories>
```

Then add the SWT dependency:
```
<dependencies>
    <dependency>
        <groupId>org.eclipse.swt</groupId>
        <artifactId>org.eclipse.swt.gtk.linux.x86_64</artifactId>
        <version>4.4</version>
    </dependency>
</dependencies>
```
Change the artifactId to match your operating system and architecture. Supported values are can be found [here](https://github.com/maven-eclipse/repo/tree/master/org/eclipse/swt).
