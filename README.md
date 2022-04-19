# MC_Test
Data analysis from MC events.

Tree files:
```
__ data
    |__ 1.Wfm.csv       -> large data file
    |__ (n+1).(n)k.csv  -> data files with (1.1<n<=0.0)
    |__ test_100.csv    -> small data file
__ sources
    |__ MC_InitialTest.ipynb    -> Initial test file for 100 events from test_100.csv file
    |__ MC_ChunkFiles.ipynb     -> Chunk large file into small files with 100 events from 1.Wfm.csv file
    |__ MC_Sanitization.ipynb   -> Clean events with error  from 1.Wfm.csv file
    |__ MC_DataAnalisys.ipynb   -> Energy analysis from 1.Wfm.csv file
    |__ MC_DataAnalisysTiming.ipynb     -> Timing analysis from 1.Wfm.csv file
    |__ 2nd file-MC_InitialTest.ipynb   -> Initial test file for 100 events from (n+1).(n)k.csv files (1.1<n<=0.0)
    |__ 2nd file-MC_Sanitization.ipynb  -> Clean events with error from (n+1).(n)k.csv files (1.1<n<=0.0)
    |__ 2nd file-MC_DataAnalisys.ipynb  -> Energy analysis from (n+1).(n)k.csv files (1.1<n<=0.0)
    |__ README.md               -> This file
__ results
    |__ test_n.csv          -> with (n>=0)
    |__ energy.csv          -> energy spectra file from 1.Wfm.csv file
    |__ 2nd_file_energy.csv -> energy spectra file from (n+1).(n)k.csv files

```

# 1- Initial test
Initial test with 100 events

# 2- Chunk files
Due to the size of the input csv file, it is necessary to split it for better data processing in pandas/numpy.
It is possible to use dask, but not implemented.

# 3- Sanitization
Clean events with errors.

# 4- Energy data analysis
Energy calculation from charge integration method.

# 5- Timing data analysis
Timing pick-off from LED, IRI and MRI methods.
