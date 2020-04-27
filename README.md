# Basic Statistics of MassBank 

Extract basic statistics from [MassBank](https://github.com/MassBank/MassBank-data). 

## Retention Time

```
grep --color=none -R RETENTION_TIME . | cut -d/ -f2 | sort -u
```

There are [30 datasets](datasets_with_retention_time.txt) for which retention time information is available. 

| Number of Spectra | Dataset | 
| --- | --- |
| 950 | AAFC |
| 5087 | Athens_Univ |
| 903 | BGC_Munich |
| 1317 | BS |
|  26 | CASMI_2012 |
| 622 | CASMI_2016 |
| 2185 | Chubu_Univ |
| 11191 | Eawag |
| 874 | Eawag_Additional_Specs |
| 340 | Fukuyama_Univ |
| 174 | GL_Sciences_Inc |
| 1118 | HBM4EU |
| 149 | IPB_Halle |
| 273 | Kazusa |
| 207 | KWR |
| 58 | MetaboLights |
| 691 | MPI_for_Chemical_Ecology |
| 79 | MSSJ |
| 621 | NAIST |
| 3756 | NaToxAq |
| 3 | Osaka_MCHRI |
| 449 | Osaka_Univ |
| 413 | PFOS_research_group |
| 10624 | RIKEN |
| 754 | RIKEN_IMS |
| 1002 | UFZ |
| 253 | Univ_Toyama |
| 2 | UPAO |
| 2626 | Washington_State_Univ |
| 2719 | Waters |
