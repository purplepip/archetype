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
    
Generate new project with

    mvn archetype:generate                      \
      -DarchetypeGroupId=com.purplepip          \
      -DarchetypeArtifactId=archetype           \
      -DarchetypeVersion=1.0.0-SNAPSHOT         \
      -DgroupId=com.purplepip                   \
      -Dversion=1.0.0-SNAPSHOT