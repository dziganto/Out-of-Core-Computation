# Out-of-Core-Computation

This repository houses five Jupyter notebooks that document my work creating an out-of-core computation + online learning pipeline. Every effort was made to make this work reproducible, including the use of random seeds where appropriate. Furthermore, the code is documented and designed in such a way that I hope many will find it useful, even if some hacking is required for your particular application. Every effort was made to eliminate bugs or mistakes. There is no guarantee that this code is bug-free, however. Use at your discretion. 

The first notebook entitled **1_Retrieve_And_Preprocess_Data.ipynb** shows how to read data directly into memory using pandas as well as how to save it to HDF5 with Blosc compression. 

The second notebook entitled **2_Train_Test_Split.ipynb** splits the raw data into training and test sets. These too are saved to HDF5. This is not necessarily required for a true online learning pipeline.

The third notebook entitled **3_Create_Multiple_Files_For_Iterating.ipynb** is not actually part of the pipeline. I merely breaks the training dataset created in the second notebook into multiple files. The point of this exerise is to show Dask's ability to handle multiple files with ease using wild card searches.

The fourth notebook entitled **4_Exploratory_Data_Analysis.ipynb** is merely included for those wanting more detail about the Higgs dataset. Basic EDA is provided. This too is not required for a true online learning pipeline, though outliers and missing values would surely cause problems.

The fifth notebook entitled **5_Online_Learning.ipynb** is the most interesting. It includes all code required to link Dask and Sklearn, creating a true out-of-core and online learning pipeline. 

---

I hope you find something useful here and if you find mistakes please let me know.
