# facebook-UDF-library

Maven compilable Facebook Hive UDF APIs collection found from Jira issue [Hive-1545][1].

## Build

``` shell
mvn package
```

This will create the executable in target directory.

## Usage

Add facebook-udfs-x.x.x-all.jar into Hive.

``` shell
hive > CREATE FUNCTION md5 as 'com.facebook.hive.udf.UDFMD5';

hive > select md5("@#789QWE");
c40a3517f12eeb416aad1037b99434e0
```

[1]: https://issues.apache.org/jira/browse/HIVE-1545