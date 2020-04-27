# BGC_Munich 

Contains also some spectra measured on a GC system.

## ```RECORD_TITLE``` 

Example: ```RECORD_TITLE: Leu-Gly-Gly; LC-ESI-QTOF; MS2; CE: 20; R=; [M+H]+```

## Number of unique Compounds

We determine the number of unique compounds by the names provided in the record-title: 

```
grep -h "RECORD_TITLE: .*; LC" *.txt | cut -d';' -f 1 | sort -u | wc -l
```

Output: 225

## ```INTERNAL_ID```

The internal ID can be used to group spectra belonging to the same compound, but measured using different
MS configurations, such as collision energy or precursor type.
