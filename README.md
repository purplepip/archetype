# TL;DR

Add the following repository to your ~/.m2/settings.xml

    <profile>
      <id>purplepip</id>
      <activation>
        <activeByDefault>true</activeByDefault>
      </activation>
      <repositories>
        <repository>
          <id>archetype</id>
          <url>https://packagecloud.io/purplepip/releases/maven2</url>
        </repository>
      </repositories>
    </profile>
    
And generate new project with

    mvn archetype:generate -DarchetypeGroupId=com.purplepip -DarchetypeArtifactId=quickstart -DarchetypeVersion=1.0.6

# Starter project

This archetype uses the [starter](https://github.com/purplepip/starter) project
to use several useful libraries to bootstrap a project for rapid development.
      