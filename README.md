<p align="center">
  <img src="assets/banner.svg" alt="Soma" width="480">
</p>

<h1 align="center">Maven</h1>

<p align="center">
  Public Maven repository for the APIs of the Soma plugins.
</p>

---

This repository is where developers get the API of a Soma plugin, so their own plugin can call it. Each jar comes with its sources and has the same version number as the plugin release it belongs to.

Any Gradle or Maven build can read the repository from its URL, without a GitHub account or token.

## Packages

- **[hider-api](https://somadocs.fr/hider/dev/):** zones that hide player identities, opened and closed by another plugin, with rules that follow the game live, such as revealing whoever holds the point.

## Requirements

- **Server:** Spigot 1.8.8
- **Java:** 21 or newer

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
