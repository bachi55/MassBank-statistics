# AAFC 

## ```RECORD_TITLE``` 

Example: ```RECORD_TITLE: Fumiquinazoline H; LC-ESI-ITFT; MS2; CE: 30; R=17500; [M+Na]+```

## Number of unique Compounds

We determine the number of unique compounds by the names provided in the record-title: 

```
grep -h RECORD_TITLE *.txt | cut -d';' -f 1 | sort -u | wc -l
```

Output: 149

If we want to distiguish also with respect to the ionization mode, we can modify the "cut" 
command: ```cut -d';' -f1,6```
