# Soma

A tiny public Maven repository: the published artifacts of [Soma](https://github.com/Sowmha)'s libraries.
The source stays private; only the compiled jars live here, and you don't need a token to grab them.

## Use a package

Point your build at the repository, then add the dependency you want.

### Gradle

```gradle
repositories {
    maven { url 'https://sowmha.github.io/maven/' }
}

dependencies {
    compileOnly 'top.soma.hider:api:1.0.0'
}
```

### Maven

```xml
<repositories>
  <repository>
    <id>soma</id>
    <url>https://sowmha.github.io/maven/</url>
  </repository>
</repositories>

<dependencies>
  <dependency>
    <groupId>top.soma.hider</groupId>
    <artifactId>api</artifactId>
    <version>1.0.0</version>
  </dependency>
</dependencies>
```

