# facebook-UDF-library

create temporary function md5 as 'com.facebook.hive.udf.UDFMD5';

hive> select md5("@#789QWE");
OK
c40a3517f12eeb416aad1037b99434e0
Time taken: 1.867 seconds, Fetched: 1 row(s)