# Releasing the dataset

## Recreate the raw data from glottography-data

In case of upstream changes in glottography-data:
```shell
cldfbench download cldfbench_eriksen2011nature.py
```

## Recreate the CLDF data

```shell
cldfbench makecldf cldfbench_eriksen2011nature.py --glottolog-version v5.2
cldfbench cldfreadme cldfbench_eriksen2011nature.py
cldfbench zenodo --communities glottography cldfbench_eriksen2011nature.py
cldfbench readme cldfbench_eriksen2011nature.py
```

## Validation

```shell
cldf validate cldf
```

```shell
cldfbench geojson.validate cldf
```

```shell
cldfbench geojson.glottolog_distance cldf --format pipe
```

| ID | Distance | Contained | NPolys |
|:---------|-----------:|:------------|---------:|
| acha1250 | 0.51 | False | 4 |
| agav1236 | 0.04 | False | 1 |
| agua1251 | 0.06 | False | 1 |
| aika1237 | 0.00 | True | 1 |
| amah1246 | 0.26 | False | 1 |
| ando1256 | 0.40 | False | 1 |
| apol1242 | 0.00 | True | 1 |
| apur1254 | 0.00 | True | 1 |
| arai1239 | 1.84 | False | 1 |
| araw1276 | 0.00 | True | 1 |
| arua1264 | 0.00 | True | 7 |
| arub1238 | 0.00 | True | 6 |
| arut1244 | 0.00 | True | 1 |
| awet1244 | 0.18 | False | 1 |
| baka1277 | 0.00 | True | 1 |
| baur1253 | 2.00 | False | 1 |
| beto1236 | 0.00 | True | 1 |
| call1235 | 0.64 | False | 1 |
| cana1260 | 0.00 | True | 1 |
| cand1248 | 0.00 | False | 2 |
| cari1279 | 0.00 | True | 1 |
| cayu1262 | 0.00 | True | 1 |
| cham1318 | 0.57 | False | 1 |
| chib1270 | 0.00 | False | 5 |
| chiq1248 | 0.00 | True | 1 |
| coca1259 | 0.00 | True | 1 |
| cofa1242 | 0.00 | False | 1 |
| east2555 | 0.00 | True | 1 |
| gali1262 | 0.00 | False | 25 |
| game1240 | 0.00 | True | 1 |
| guah1255 | 0.00 | True | 5 |
| guam1236 | 0.00 | True | 1 |
| igna1246 | 0.00 | False | 1 |
| iran1263 | 0.46 | False | 1 |
| iton1250 | 0.00 | False | 1 |
| kama1373 | 0.19 | False | 1 |
| kano1245 | 1.62 | False | 1 |
| kari1317 | 0.00 | True | 1 |
| kaya1329 | 0.00 | True | 1 |
| kaya1330 | 4.29 | False | 1 |
| kuik1246 | 0.21 | False | 2 |
| kust1238 | 1.79 | False | 1 |
| kwaz1243 | 0.46 | False | 1 |
| leco1242 | 0.13 | False | 1 |
| macu1259 | 2.13 | False | 1 |
| maku1246 | 4.82 | False | 1 |
| mana1299 | 0.00 | False | 6 |
| mapi1252 | 0.22 | False | 1 |
| mara1408 | 1.89 | False | 4 |
| mari1442 | 0.00 | True | 1 |
| mati1253 | 0.75 | False | 1 |
| mehi1240 | 0.47 | False | 1 |
| miar1236 | 0.11 | False | 1 |
| mose1249 | 0.19 | False | 1 |
| movi1243 | 0.16 | False | 1 |
| mund1330 | 2.60 | False | 1 |
| muni1258 | 0.31 | False | 1 |
| ocai1244 | 0.77 | False | 1 |
| omag1248 | 0.00 | True | 1 |
| omur1241 | 0.47 | False | 1 |
| opon1234 | 0.32 | False | 1 |
| otom1301 | 0.00 | True | 1 |
| paez1247 | 3.40 | False | 2 |
| pali1279 | 0.07 | False | 1 |
| pana1306 | 0.12 | False | 1 |
| para1310 | 1.18 | False | 1 |
| pare1272 | 0.00 | True | 1 |
| piap1246 | 1.27 | False | 1 |
| piar1243 | 0.46 | False | 1 |
| pija1235 | 1.85 | False | 1 |
| pira1253 | 0.00 | True | 4 |
| puin1248 | 0.95 | False | 2 |
| pume1238 | 0.00 | True | 1 |
| puqu1242 | 1.19 | False | 1 |
| rikb1245 | 0.82 | False | 1 |
| sali1298 | 1.34 | False | 2 |
| sara1331 | 1.77 | False | 1 |
| ship1254 | 0.00 | True | 1 |
| shua1257 | 0.00 | True | 1 |
| siri1273 | 0.00 | True | 1 |
| tapi1254 | 0.16 | False | 1 |
| taru1236 | 0.00 | True | 2 |
| taus1253 | 0.04 | False | 1 |
| tere1279 | 0.00 | False | 5 |
| ticu1245 | 0.00 | True | 1 |
| timo1237 | 1.06 | False | 1 |
| tora1263 | 1.83 | False | 1 |
| trum1247 | 0.01 | False | 1 |
| urar1246 | 0.00 | True | 1 |
| wany1246 | 0.00 | True | 7 |
| waor1240 | 0.00 | True | 2 |
| wapi1253 | 0.00 | True | 1 |
| wara1303 | 0.74 | False | 9 |
| waur1244 | 0.98 | False | 1 |
| waya1270 | 0.00 | True | 1 |
| yano1262 | 0.00 | True | 3 |
| yawa1261 | 0.00 | True | 1 |
| yine1238 | 0.00 | True | 1 |
| yukp1241 | 0.00 | True | 1 |
| yura1255 | 0.09 | False | 1 |
| zapa1253 | 0.03 | False | 2 |

```shell
cldfbench geojson.glottolog_distance cldf --format tsv | csvformat -t | csvgrep -c Distance -r"^0\.?" -i | csvsort -c Distance | csvcut -c ID,Distance | csvformat -E | termgraph
```

```
timo1237: ▇▇▇▇▇▇▇▇▇▇ 1.06 
para1310: ▇▇▇▇▇▇▇▇▇▇▇▇ 1.18 
puqu1242: ▇▇▇▇▇▇▇▇▇▇▇▇ 1.19 
piap1246: ▇▇▇▇▇▇▇▇▇▇▇▇▇ 1.27 
sali1298: ▇▇▇▇▇▇▇▇▇▇▇▇▇ 1.34 
kano1245: ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 1.62 
sara1331: ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 1.77 
kust1238: ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 1.79 
tora1263: ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 1.83 
arai1239: ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 1.84 
pija1235: ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 1.85 
mara1408: ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 1.89 
baur1253: ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 2.00 
macu1259: ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 2.13 
mund1330: ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 2.60 
paez1247: ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 3.40 
kaya1330: ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 4.29 
maku1246: ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 4.82 
```
