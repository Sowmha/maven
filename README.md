# Soma

A tiny public Maven repository: the published artifacts of [Soma](https://github.com/Sowmha)'s libraries.
The source stays private; only the compiled jars live here, and you don't need a token to grab them.

## Packages

| Artifact | What it is |
|---|---|
| `top.soma:hider-api` | Public API of SomaHider: hide players inside a zone behind composable visibility rules. |

## Use a package

Point your build at the repository, then add the dependency you want.

### Gradle

```gradle
repositories {
    maven { url 'https://sowmha.github.io/maven/' }
}

dependencies {
    compileOnly 'top.soma:hider-api:1.13.3'
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
    <groupId>top.soma</groupId>
    <artifactId>hider-api</artifactId>
    <version>1.13.3</version>
    <scope>provided</scope>
  </dependency>
</dependencies>
```
