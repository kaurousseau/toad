# TOAD

## Running TOAD

Once the imaging data are converted, you simply have to run the command 'toad' from the folder that contains the converted files:

~~~bash
# Go to the data-containing folder
cd toad_data

# Run TOAD
toad *
~~~

Data preprocessing for one subject takes about 2 days to complete. 
Parallel processing on multiple subjects or large dataset is also possible on the UNF servers, depending on their work load at the given time. 

## Verification

One can know the progress of the preprocessing (e.g. how many subjects have been preprocessed) on the UNF servers by simply typing the command 'qstat'.

Once the work is finished, you will find a new set of folders under each subject's directory.
These folders contain the dataset, masks, and images generated by TOAD's preprocessing pipeline. The results can be quickly verified thanks to QA…

<!-- FIXME QA -->
*Section à développer*

In case of any problem, check the log files under the folder 'log', which can be found in each subject that has been preprocessed by TOAD:

~~~bash
# Replace 'toad_data' below by the name of the folder used during data convertion. 
cd toad_data/subject_name/99-logs

# List all available logs
ls

# To consult a log file, for example 'results.log'
vi results.log
~~~





