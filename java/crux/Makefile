.PHONY: clean pkg deps run

pkg:
	mvn --quiet package
	cp target/crux-1.0-SNAPSHOT.jar ../../inst/java

clean:
	mvn clean

deps:
	mvn dependency:copy-dependencies -DoutputDirectory=../../inst/java

new:
	mvn archetype:generate -DgroupId=is.rud.crux -DartifactId=crux -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false && mv Makefile crux
