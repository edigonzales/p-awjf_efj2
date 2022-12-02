# p-awjf_efj2

```
java -jar /Users/stefan/apps/ili2gpkg-4.8.0/ili2gpkg-4.8.0.jar --dbfile ch.so.awjf.jagdreviergrenzen_efj2.gpkg --strokeArcs --defaultSrsCode 2056 --nameByTopic --createMetaInfo --createGeomIdx --models SO_AWJF_Jagdreviergrenzen_EFJ2_20220811 --modeldir ".;https://models.geo.admin.ch" --schemaimport
```

Copy/Paste in QGIS

```
java -jar /Users/stefan/apps/ili2gpkg-4.8.0/ili2gpkg-4.8.0.jar --dbfile ch.so.awjf.jagdreviergrenzen_efj2.gpkg  --models SO_AWJF_Jagdreviergrenzen_EFJ2_20220811 --modeldir ".;https://models.geo.admin.ch" --export ch.so.awjf.jagdreviergrenzen_efj2.xtf
```

```
java -jar /Users/stefan/apps/ilivalidator-1.11.15-SNAPSHOT/ilivalidator-1.11.15-SNAPSHOT.jar ch.so.awjf.jagdreviergrenzen_efj2.xtf
```


Version 2:

```
java -jar /Users/stefan/apps/ili2gpkg-4.8.0/ili2gpkg-4.8.0.jar --dbfile ch.so.awjf.gebiete_efj2.gpkg --strokeArcs --defaultSrsCode 2056 --nameByTopic --createMetaInfo --createGeomIdx --models SO_AWJF_Rahmenmodell_EFJ2_20220818 --modeldir ".;https://models.geo.admin.ch" --schemaimport
```

Copy/Paste in QGIS

```
java -jar /Users/stefan/apps/ili2gpkg-4.8.0/ili2gpkg-4.8.0.jar --dbfile ch.so.awjf.gebiete_efj2.gpkg  --models SO_AWJF_Rahmenmodell_EFJ2_20220818 --modeldir ".;https://models.geo.admin.ch" --export ch.so.awjf.gebiete_efj2_20221004.xtf
```

```
java -jar /Users/stefan/apps/ilivalidator-1.11.15-SNAPSHOT/ilivalidator-1.11.15-SNAPSHOT.jar ch.so.awjf.gebiete_efj2.xtf
java -jar /Users/stefan/apps/ilivalidator-1.11.15-SNAPSHOT/ilivalidator-1.11.15-SNAPSHOT.jar ch.so.awjf.gebiete_efj2_20221004.xtf
```


Wegen Fischereireviere nun mit PostgreSQL:

```
java -jar /Users/stefan/apps/ili2pg-4.9.0/ili2pg-4.9.0.jar --dbschema awjf_efj2_gebiete --dbhost localhost --dbport 54321 --dbdatabase edit --dbusr ddluser --dbpwd ddluser --strokeArcs --defaultSrsCode 2056 --nameByTopic --createMetaInfo --createGeomIdx --models SO_AWJF_Rahmenmodell_EFJ2_20220818 --modeldir ".;https://models.geo.admin.ch" --doSchemaImport --import ch.so.awjf.gebiete_efj2.xtf

java -jar /Users/stefan/apps/ili2pg-4.9.0/ili2pg-4.9.0.jar --dbschema awjf_efj2_gebiete --dbhost localhost --dbport 54321 --dbdatabase edit --dbusr ddluser --dbpwd ddluser --strokeArcs --defaultSrsCode 2056 --nameByTopic --createMetaInfo --createGeomIdx --models SO_AWJF_Rahmenmodell_EFJ2_20220818 --modeldir ".;https://models.geo.admin.ch" --export ch.so.awjf.gebiete_efj2_20221103.xtf


```


```
curl --insecure -i -X POST -F file=@ch.so.awjf.gebiete_efj2_20221103.xtf -F valid_from=2022-12-02 https://efj-services-i.verw.rootso.org/webapi/api/geo/geodata
```