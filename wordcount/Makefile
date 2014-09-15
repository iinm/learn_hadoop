all: jar

jar: class
	jar cvf ../wordcount.jar -C wordcount.classes .

class: WordCount.java
	javac -cp $(hadoop classpath) -d wordcount.classes WordCount.java

clean:
	rm -rf wordcount.classes/*
