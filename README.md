# Dataset-used-to-build-the-time-series-prediction-models
This is the modified dataset from the original rnd Bitbrains traces dataset 
To build our proposed predictive model, a publicly available workload traces, named rnd trace has been used. 
Due to the unavailability of real dataset of vehicles’ workload, we used a dataset of the observed workload of different VMs 
host on cloud computing data which is collected from a typical data centre managed by a service provider called Bitbrains 
which specializes in hosting and business computation management for enterprises. 
This dataset is a recording time series data of eleven attributes, timestamp, CPU cores, CPU capacity provisioned in MHz, CPU usage in MHz, the percentage of CPU usage, memory capacity provisioned, memory used, hard disk reading speed, hard disk writing speed, network received throughput [KB/s] and network transmitted throughput [KB/s], in frequency of 5 minutes for an interval of one month. We modified this dataset to suites our models as following: 
•	Some of the attributes have been modified: timestamp attribute has been converted from Epoch to datetime and an ID column has been added to be used as an identifier for each VM. 
•	Only two columns have been used to train our model; the percentage of CPU utilization column and memory used column. 
•	We use a frequency of 15 minutes instead of 5 minutes as this is the lowest frequency that can be accepted by Azure platform to build the prediction models. 
•	This dataset This dataset is split into two files, CPU utilization file and memory usage file. 
