# CALCITE-5300

The project contains a minimal maven project reproducing the issue reported under [CALCITE-5300](https://issues.apache.org/jira/browse/CALCITE-5300).

## Environment

```
mvn -version
Apache Maven 3.6.3 (cecedd343002696d0abb50b32b541b8a6ba2883f)
Maven home: XX
Java version: 1.8.0_261, vendor: Oracle Corporation, runtime: /opt/jdks/jdk1.8.0_261/jre
Default locale: en_US, platform encoding: UTF-8
OS name: "linux", version: "5.4.0-126-generic", arch: "amd64", family: "unix"
```

## Steps to reproduce

To reproduce the problem run:
```
mvn clean install
```

The error is the following:
```
[ERROR] Failed to execute goal org.apache.maven.plugins:maven-compiler-plugin:3.1:compile (default-compile) on project immutables-calcite-problem: Compilation failure
[ERROR] cannot access org.immutables.value.Value
[ERROR]   class file for org.immutables.value.Value not found
```

