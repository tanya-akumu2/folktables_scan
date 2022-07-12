# Scanning folktables data

This repo contains the materials for applying subset scanning on folktables data. This data is downloaded from the [Folktables Python package](https://github.com/zykls/folktables), preprocessed and downloaded to the folder.

## Downloading the data

To download and preprocess the data, run the folktable_preprocessing.ipynb file. This will download the US cencus Income data, extract feature values and map the codes to their string values. After the mapping, the dataframe is saved as a csv file in the folder.

## Running the Scanning Algorithm

We use the MDSS scanning algorithm from the open sourced [AIF360 toolkit](https://github.com/Trusted-AI/AIF360/tree/master/aif360/detectors). The datasets downloaded from the previous test is what scan. Run the folktables_scan.ipynb to scan and view the results

## Setup
```
# create virtual env
python -m venv aif360
# activate it (if using windows, see note below)
source aif360/bin/activate

# install packages
pip install -r requirements.txt
```

You can then run the [folktables_preprocessing.ipynb](https://github.com/tanya-akumu2/folktables_scan/blob/main/folktable_preprocessing.ipynb) notebook to download and save data from folktables or run the [folktables_scan.ipynb](https://github.com/tanya-akumu2/folktables_scan/blob/main/folktables_scan.ipynb) to run the scanning algorithm on the downloaded data. You can also specify which year to download (between 2014-2018) by specifying the `survey_year` parameter in the preprocessing notebook


## Useful links:

[AIF360 Toolkit](https://github.com/Trusted-AI/AIF360)
[More examples using MDSS](https://github.com/Trusted-AI/AIF360/blob/master/examples/demo_mdss_detector.ipynb)
[MDSS Paper](https://arxiv.org/abs/1611.08292)