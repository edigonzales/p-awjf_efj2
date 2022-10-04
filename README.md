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