# Using Graddle Kotlin

- Add repository to your `build.gradle.kts`
  ```kts
  repositories {
      maven {
          url = uri("https://raw.githubusercontent.com/tncrazvan/artifacts/main")
          metadataSources {
              mavenPom()
              artifact()
              ignoreGradleMetadataRedirection()
          }
      }
  }
  ```

- Add the library to your `build.gradle.kts`, for example `dev.razshare.unsafe`
  ```kts
  dependencies {
      implementation("dev.razshare:unsafe:1.0.0")
  }
  ```

# Using Maven

- Add repository to your `pom.xml`
  ```xml
  <repositories>
      <repository>
          <id>dev.razshare</id>
          <url>https://raw.githubusercontent.com/tncrazvan/artifacts/main</url>
      </repository>
  </repositories>
  ```

- Add the library toy our `pom.xml`, for example `dev.razshare.unsafe`
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
