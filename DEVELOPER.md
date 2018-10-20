# Release Procedure

Build pipeline builds releases and deploys to package repository for tagged 
releases. This can be triggered with :

    mvn release:prepare && mvn release:clean

# Template to archetype source

Maintain the archetype-template project as template to validate the archetype.
Then create an archetype from this template with

    mvn archetype:create-from-project -pl archetype-template
    
And look in archetype-template/target/generated-sources/archetype/ for the 
appropriate archetype source that should be moved into the actual archetype
for build and release.
  
    