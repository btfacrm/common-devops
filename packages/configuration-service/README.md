# Alternative XML Parser
The action uses XMLScarlet to get the main values from pom.xml.

Another parser is XmlLint, next is the syntax to query the pom.xml

servicename=$( xmllint --xpath "//*[local-name()='project']/*[local-name()='name']/text()" pom.xml)
serviceversion=$( xmllint --xpath "//*[local-name()='project']/*[local-name()='version']/text()" pom.xml)
servicegroup=$( xmllint --xpath "//*[local-name()='project']/*[local-name()='groupId']/text()" pom.xml)
serviceartifact=$( xmllint --xpath "//*[local-name()='project']/*[local-name()='artifactId']/text()" pom.xml)
