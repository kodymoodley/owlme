*owl-me for OWLAPI v5*
====

#### a Java-based module extractor for OWL ontologies

Built using the [OWL API](https://github.com/owlcs/owlapi). This is an updated version of [owl-me](https://github.com/rsgoncalves/module-extractor) for use with OWL API version 5. In other words, this version will generate modules that can be loaded with Protege 5 (i.e., [Protege Desktop](https://github.com/protegeproject/protege)).

All credit goes to [Rafael Goncalves](https://github.com/rsgoncalves) who developed the original tool.

#### For Users: Installing and using the tool

Requirements:

+ Java Runtime Environment 1.8+
+ An OWL ontology (.owl file)
+ A CSV file containing a list of ontology terms (one on each line)

Steps:

1. Download the latest .jar file from the [releases](https://github.com/kodymoodley/owlme/releases) section of this repository.

2. Double click the .jar file to open the tool. Alternatively, from the commandline, execute:

`java -jar -Xmx4G -DentityExpansionLimit=100000000 owl-me-${version}.jar`

3. Load your input ontology and signature file

4. Select a location to save the output module, and click on the "Extract Module" button.

#### For Developers: Building the tool from source

Requirements:

+ Apache's [Maven](http://maven.apache.org/index.html).
+ A tool for checking out a [Git](http://git-scm.com/) repository.
+ Java JDK 1.8+

Steps:

1. Get a copy of the code:

        git clone https://github.com/kodymoodley/owlme.git
    
2. Change into the `owlme/` directory.

3. Type `mvn clean package`.  On build completion, the `target/` directory will contain an `owl-me-${version}.jar` file.

#### License

This version of owl-me is released under the [GNU Lesser General Public License Version 3](https://www.gnu.org/licenses/lgpl-3.0.txt). The original [owl-me](https://github.com/rsgoncalves/module-extractor) is developed by [Rafael Goncalves](https://github.com/rsgoncalves) and released under the same license.




 
