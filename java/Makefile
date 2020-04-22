clean:
	@echo clean
	[ -f Hello.class ] && rm Hello.class || true
	[ -f Hello.jar ] && rm Hello.jar || true

compile: clean
	@echo compile
	javac Hello.java

run-local: compile
	@echo run
	java Hello

build: compile
	jar cfm Hello.jar Manifest.txt Hello.class

run: build
	java -jar Hello.jar