# How to use

Add repository to your pom.xml

```xml
<repositories>
    <repository>
        <id>dev.razshare</id>
        <url>https://raw.githubusercontent.com/tncrazvan/artifacts/main</url>
    </repository>
</repositories>
```

Then add your dependency, for example `dev.razshare.unsafe`

```xml
<dependencies>
    <dependency>
        <groupId>dev.razshare</groupId>
        <artifactId>unsafe</artifactId>
        <version>1.0.0</version>
        <type>jar</type>
    </dependency>
</dependencies>
```

and obviously run

```sh
mvn install
```

Final result

```kt
import dev.razshare.unsafe.ok

fun main() {
    val result = ok("hello world")
}
```