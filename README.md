# DSPS24

## Data Science for Pavements Symposium (DSPS)

This is the third DSPS student competition on the application of AI for pavement condition monitoring. Participants will use novel machine learning algorithms to predict the pavement condition index (PCI) for road sections based on images captured from infrastructure - mounted sensors. Training datasets provided consists of Top-down views of pavement image data and associated pavement condition index. Participants are free to annotate training datasets and use any model architecture to predict the PCI of the road section.

 <div >
    <a>
     <img src="https://github.com/UM-Titan/DSPS24/blob/main/dsps.png" width="100%"/>
    </a>
    <a>
     <img src="https://github.com/UM-Titan/DSPS24/blob/main/11177_%5B40.72135599531271%2C%20-89.44741236557417%5D_%202023-10-18%2020-36-50_24.2979_LD.jpg" width="25%"/>
    </a>
  <a>
     <img src="https://github.com/UM-Titan/DSPS24/blob/main/17429_%5B40.70484625151038%2C%20-89.44938348689516%5D_%202023-10-20%2018-38-59_51.63905_LD.jpg" width="25%"/>
    </a>
  <a>
     <img src="https://github.com/UM-Titan/DSPS24/blob/main/399_(40.7199438333333%2C%20-89.424166)_%202023-10-18%2015-43-34_55.86445_D.jpg" width="24%"/>
    </a>
  <a>
     <img src="https://github.com/UM-Titan/DSPS24/blob/main/399_(40.7199438333333%2C%20-89.42___4166)_%202023-10-18%2015-43-34_55.86445_D.jpg" width="24%"/>
    </a>
</div> 

## <summary>TIMELINE </summary>
* 12-11-2023: Team registration begins! Challenge GitHub page and Website opens.
* 12-20-2023: Training data for competition is released. Download data from GitHub page
* 01-08-2024: Test Data for competition is released.
* 01-22-2024: Leaderboard website is open for results submission.
* 02-09-2024: Tutorial on how to use benchmark model.
* 02-12-2024: The link for submitting the source code enabled.
* 02-23-2024: Competition ends! Deadline for submitting the source code & the solutions.
* 02-26-2024: Top 5 teams shortlisted for paper submission!
* 03-05-2024: Top 3 winners announced
* 03-11-2024: Symposium begins!

## <summary> RULES </summary>
We expect you to respect the spirit of the competition and do not cheat.
* There are no restrictions on the size of teams.
* The use of external data for model training is forbidden.
* Pre-trained models are allowed in the competition.
* Teams are free to use any model architecture of their choice. 
* Please submit source code and trained model before the deadline. IPython Notebook is desirable for the source code submission. The organizers will verify the reproducibility of the algorithm before determining the final winner.


# Data Download
```bash
## use gdown in google collab to download training data. 
!gdown --id '1zg5EDls7E4ZnkWzPKh_XNkw564ns22mq'
```

## Data Extraction 
```bash
## use unzip in google collab to extract zipped training data to current directory. 
!unzip 'data.zip' -d './'
```

## Test Data Download
```bash
## use gdown in google collab to download the test data.
## if gdown fails, click on output link from gdown to download data directly from browser

!gdown --id '1KdNjCIot9SYh9JxRHuCjrPdmgUDazZ9U'
```

## Generate Submission File
```bash
## use code below to generation JSON formated data for submission.
## The code below takes in a dataframe with two columns: image_name and PCI
 
import pandas as pd
import json
# df: should have two columns - image_name and PCI
def gen_submit(df):
  out_json = []
  for idx, results in df.iterrows():
    out_json.append({results['image_name']:results['PCI']})
  with open('submission.json', 'w') as f:
    json.dump(out_json, f)

```
