# infrastructure_lab

-[problema](https://community.sonatype.com/t/i-removed-local-authenticating-realm-by-accident-how-to-recover/4463)
-[solucion](https://support.sonatype.com/hc/en-us/articles/213467158-How-to-reset-a-forgotten-admin-password-in-Nexus-3-x)


## stop nexus
- [reference](https://help.sonatype.com/repomanager3/high-availability/operating-your-cluster#Operatingyourcluster-Shutdown)

```
cd /opt/sonatype/nexus/bin/
./nexus stop
```
## backup

```
cd nexus-data/
cp -r -a ./db ./db_backup
```

## connect to database
```
cd opt/sonatype/nexus/lib/support/
java -jar ./nexus-orient-console.jar

CONNECT plocal:/nexus-data/db/security admin admin
```



 CONNECT REMOTE:localhost admin admin

  CONNECT remote:localhost admin admin


  CONNECT remote:localhost admin 

  Bee$ion1234

  CONNECT plocal:/nexus-data/db/component admin admin

  security admin admin


 select * from realm
+----+-----+------+----------------------+
|#   |@RID |@CLASS|realm_names           |
+----+-----+------+----------------------+
|0   |#40:0|realm |[NpmToken,DockerToken]|
+----+-----+------+----------------------+



  
