A Maven repository hosting SWT and JFace jar files / artefacts which can't be found in maven central.

### SWT example

Add this repository to your project's pom.xml:

```
<repositories>
    <repository>
        <id>swt-repo</id>
        <url>https://raw.githubusercontent.com/maven-eclipse/repo/master/</url>
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
