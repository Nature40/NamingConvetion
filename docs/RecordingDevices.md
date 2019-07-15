# Naming conventions in Nature 4.0 for measurement recording entities (Draft)

This convention assigns unique IDs to recordings in a hierarchical structure. Location of measurements is explicitly not encoded in the ID, to allow exchange of devices between locations. 

Location (e.g. core study tree) and other meta data is will be associated with that IDs. Meta data includes validity periods of time (start and end timestamp) to specify variables of current measurement (e.g. over time one device measures at two different core study trees).

meta data example:

ID|start|end|location
------------ | ------------- | ------------- | -------------
id1|*|2019-04-01T17:01|cst_001
id1|2019-05-05T10:00|2019-05-15T12:00|cst_002
id1|2019-05-15T14:00|*|cst_003

---
### Three-character string for the study area
```
mof
``` 

---
### Three-character string for the data collecting device type (not measuring device)
```
mof_aaa
mof_bbb
```

---
### Three-digit number sequence for ongoing numbering
This numbers the individual collecting devices. Numbers are unique within on device type. If one device is replaced by a new device, a new number is assigned.
```
mof_aaa_001
mof_aaa_002
mof_bbb_001
mof_bbb_002
```

---
### Three-character string for the measuring device type
Measuring devices are connected to one collecting device
```
cbh
cbv
```

---
### Three-digit number sequence for ongoing numbering
This numbers the individual measuring devices. 

(?) Numbers are unique for each measuring device type at one collecting device (?)
```
mof_aaa_001_cbh_001
mof_aaa_001_cbh_002
mof_aaa_001_cbv_001
mof_aaa_001_cbv_002
mof_bbb_002_cbh_001
mof_bbb_002_cbh_002
mof_bbb_002_cbv_001
mof_bbb_002_cbv_002
```

OR (?) Numbers are unique for each measuring device type over all collecting devices (?)

```
mof_aaa_001_cbh_001
mof_aaa_001_cbh_002
mof_aaa_001_cbv_001
mof_aaa_001_cbv_002
mof_bbb_002_cbh_003
mof_bbb_002_cbh_004
mof_bbb_002_cbv_003
mof_bbb_002_cbv_004
```

---
### Two-character string for the sensor measurement type
```
mof_aaa_001_cbh_001_ta
mof_aaa_001_cbh_001_rH
mof_bbb_002_cbh_001_ta
mof_bbb_002_cbh_001_rH
```

---
### Two-digit number sequence for ongoing numbering

(?) Numbers are unique for each measuring device type at one measuring device (?)
```
mof_aaa_001_cbh_001_ta_01
mof_aaa_001_cbh_001_ta_02
mof_aaa_001_cbh_001_rH_01
mof_aaa_001_cbh_001_rH_02
mof_bbb_002_cbh_001_ta_01
mof_bbb_002_cbh_001_ta_02
mof_bbb_002_cbh_001_rH_01
mof_bbb_002_cbh_001_rH_02
```

OR (?) Numbers are unique at measuring device independent of sensor measurement type (?)
```
mof_aaa_001_cbh_001_ta_01
mof_aaa_001_cbh_001_ta_02
mof_aaa_001_cbh_001_rH_03
mof_aaa_001_cbh_001_rH_04
mof_bbb_002_cbh_001_ta_01
mof_bbb_002_cbh_001_ta_02
mof_bbb_002_cbh_001_rH_03
mof_bbb_002_cbh_001_rH_04
```
