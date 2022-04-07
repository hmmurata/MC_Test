# MC_Test
Tree files:
__ data
    |__ 1.Wfm.csv
__ sources
    |__ MC_InitialTest.ipynb    -> Initial test file for 100 events 
    |__ MC_ChunkFiles.ipynb     -> Chunk large file into small files with 100 events
    |__ MC_Sanitization.ipynb   -> 
    |__ README.md
__ results
    |__ test_n.csv              with n>=0



# 1- Chunk files
Due to the size of the input csv file, it is necessary to split it for better data processing.
Use MC_ChunkFiles.ipynb to chunk files:
Example:
Input: ../data/1.Wfm.csv
Output: ../results/test_n.csv  n>=0

# 2- 