# sb-assembly-descriptors
SB maven assembly descriptors

This project contains our most useful assembly descriptors. It is meant to reduce the amount of boilerplate code to
maintain in our project.

Currently, there are 5 descriptors

 * webapp+conf-in-*.xml: These descriptors package everything in src/main/config in /conf, and all webapps you depend on
 in /webapps, along with README.md and CHANGELOG.md
 * java-command-line.xml: The standard assembly descriptor for command line java applications. Package src/main/scripts
 go in /bin, all runtime dependencies go in /lib and src/main/config go in /conf. Permissions are set correctly. Config and scripts
 are filtered
 * Appassembler-*.xml: package the app assembler folder