# TestContainers MS SQL Server Module

Testcontainers module for the MS SQL Server database.

See [testcontainers.org](https://www.testcontainers.org) for more information about Testcontainers.

## Usage example

Running MS SQL Server as a stand-in for in a test:

```java
public class SomeTest {

    @Rule
    public MSSQLServerContainer mssqlserver = new MSSQLServerContainer();
    
    @Test
    public void someTestMethod() {
        String url = mssqlserver.getJdbcUrl();

        ... create a connection and run test as normal
```

## License

See [LICENSE](LICENSE).

## Copyright

Copyright (c) 2017 - 2019 G DATA Software AG and other authors.

See [AUTHORS](AUTHORS) for contributors.