# Athens_Univ 

Contains also some spectra measured on a GC system.

## ```RECORD_TITLE``` 

Example: ```RECORD_TITLE: alpha-Hydroxymidazolam; LC-ESI-QTOF; MS2; CE: Ramp 22.1-33.2 eV; R=35000; [M+H]+```

## Number of unique Compounds

We determine the number of unique compounds by the names provided in the record-title: 

```
grep -h "RECORD_TITLE: .*; LC" *.txt | cut -d';' -f 1 | sort -u | wc -l
```

Output: 861

## ```INTERNAL_ID```

The internal ID can be used to group spectra belonging to the same compound, but measured using different
MS configurations, such as collision energy or precursor type.
