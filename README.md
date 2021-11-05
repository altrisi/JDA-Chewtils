## JDA-Chewtils
JDA-Chewtils is a fork of [JDA-Utilities](https://github.com/JDA-Applications/JDA-Utilities) which is a series of tools and utilities for use with [JDA](https://github.com/DV8FromTheWorld/JDA) to assist in bot creation.

## Support

If you're needing help or want to help, feel free to hop onto the [#jda-chewtils](https://discord.gg/SUGVxJpg8r) channel on my server. 

Please do NOT use the official JDA server for help with this fork.

## Packages

Since JDA-Utilities 2.x, the library has been split into multiple modular projects,
in order to better organize its contents based on what developers might want to use and not use.

+ [Command Package](https://github.com/Chew/JDA-Chewtils/tree/master/command)
+ [Commons Package](https://github.com/Chew/JDA-Chewtils/tree/master/commons)
+ [CommandDoc Package](https://github.com/Chew/JDA-Chewtils/tree/master/doc)
+ [Examples Package](https://github.com/Chew/JDA-Chewtils/tree/master/examples)
+ [Menu Package](https://github.com/Chew/JDA-Chewtils/tree/master/menu)

Visit individual modules to read more about their contents!

## Getting Started
You will need to add this project as a dependency (either from the latest .jar from the releases page, 
or via maven or gradle), as well as [JDA](https://github.com/DV8FromTheWorld/JDA). 

With maven:
```xml
  <dependency>
    <groupId>pw.chew</groupId>
    <artifactId>jda-chewtils</artifactId>
    <version>JDA-CHEWTILS-VERSION</version>
    <scope>compile</scope>
    <type>pom</type>
  </dependency>
  <dependency>
    <groupId>net.dv8tion</groupId>
    <artifactId>JDA</artifactId>
    <version>JDA-VERSION</version>
  </dependency>
```
```xml
  <!-- Chew's Maven Repo for JDA-Chewtils -->
  <repository>
    <id>chew</id>
    <name>m2-chew</name>
    <url>https://m2.chew.pro/releases</url>
  </repository>
  <!-- JDA repo to get JDA -->
  <repository>
    <id>dv8tion</id>
    <name>m2-dv8tion</name>
    <url>https://m2.dv8tion.net/releases</url>
  </repository>
```

With gradle:
```groovy
dependencies {
    compile 'pw.chew:jda-chewtils:JDA-UTILITIES-VERSION'
    compile 'net.dv8tion:JDA:JDA-VERSION'
}

repositories {
    mavenCentral() // for transitive dependencies
    // for JDA
    maven {
      name 'm2-dv8tion'
      url 'https://m2.dv8tion.net/releases'
    }
    // For JDA-Chewtils
    maven { url "https://m2.chew.pro/releases" }
}
```

Individual modules can be downloaded using the same structure shown above, with the addition of the module's
name as a suffix to the dependency:

With maven:
```xml
  <dependency>
    <groupId>pw.chew</groupId>
    <!-- Notice that the dependency notation ends with "-command" -->
    <artifactId>jda-chewtils-command</artifactId>
    <version>JDA-CHEWTILS-VERSION</version>
    <scope>compile</scope>
  </dependency>
```

With gradle:
```groovy
dependencies {
    // Notice that the dependency notation ends with "-command"
    compile 'pw.chew:jda-chewtils-command:JDA-CHEWTILS-VERSION'
}
```

## Examples

Guides and information can be found on the [wiki](https://github.com/Chew/JDA-Chewtils/wiki).

