This example demonstrates:

Unit tests written with JUnit 4
Unit test using PowerMockito to mock classes and test System.exit()
Integration tests written with JUnit 4
Integration test using system-rules to test System.out
Code coverage reports via Cobertura
A Maven build that puts it all together
Running the tests
To run the unit tests, call mvn test
To run the integration tests as well, call mvn verify
To generate (unit test) code coverage reports, call mvn cobertura:cobertura, and point a browser at the output in target/site/cobertura/
Conventions
This example follows the following basic conventions:

| unit test | integration test --- | --- | --- resides in: | src/test/java/*Test.java | src/test/java/*IT.java executes in Maven phase: | test | verify handled by Maven plugin: | surefire | failsafe


sample commit
