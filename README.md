# Scanning folktables data

This repo contains the materials for applying subset scanning on folktables data. This data is downloaded from the [Folktables Python package](https://github.com/zykls/folktables), preprocessed and downloaded to the folder.

## Downloading the data

To download and preprocess the data, run the folktable_preprocessing.ipynb file. This will download the US cencus Income data, extract feature values and map the codes to their string values. After the mapping, the dataframe is saved as a csv file in the folder.

## Running the Scanning Algorithm

We use the MDSS scanning algorithm from the open sourced [AIF360 toolkit](https://github.com/Trusted-AI/AIF360/tree/master/aif360/detectors). The datasets downloaded from the previous test is what scan. Run the folktables_scan.ipynb to scan and view the results

