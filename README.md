## Overview

The documentation is written in the Asciidoctor format, and processed using the Maven Asciidoctor plugin.

## Prerequisites ##

You need to have Maven 3.0.5 or later installed on your machine.

## Building the documentation project ##

`mvn clean install` will build the documentation and create a static website in `target/generated-docs`. 

The build process will also create files for all Karaf commands based on the correct Karaf version defined in the pom file. 
It appears that the Karaf manual is no longer deployed as a Maven artifact to the central repository. Consequently, no copy of the user and developmemt guides are included in this documentation. Instead, the link to the current Karaf documentation is provided.
  
## Publishing the documentation to the website ##

If you're an Apache ServiceMix committer, you can publish a new copy of the documentation pages with this command:

`mvn clean install scm-publish:publish-scm`  
