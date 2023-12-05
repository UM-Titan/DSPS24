# DSPS24

## Data Science for Pavements Symposium (DSPS)

This is the third DSPS student competition on the application of AI for pavement condition monitoring. Participants will use novel machine learning algorithms to predict the pavement condition index (PCI) for road sections based on images captured from infrastructure - mounted sensors. Training datasets provided consists of Top-down views of pavement image data and associated pavement condition index. Participants are free to annotate training datasets and use any model architecture to predict the PCI of the road section.

 <div >
    <a>
     <img src="https://github.com/UM-Titan/DSPS24/blob/main/dsps.png" width="100%"/>
    </a>
    <a>
     <img src="https://github.com/UM-Titan/DSPS24/blob/main/11177_%5B40.72135599531271%2C%20-89.44741236557417%5D_%202023-10-18%2020-36-50_24.2979_LD.jpg" width="20%"/>
    </a>
  <a>
     <img src="https://github.com/UM-Titan/DSPS24/blob/main/17429_%5B40.70484625151038%2C%20-89.44938348689516%5D_%202023-10-20%2018-38-59_51.63905_LD.jpg" width="20%"/>
    </a>
  <a>
     <img src="https://github.com/UM-Titan/DSPS24/blob/main/399_(40.7199438333333%2C%20-89.424166)_%202023-10-18%2015-43-34_55.86445_D.jpg" width="20%"/>
    </a>
  <a>
     <img src="https://github.com/UM-Titan/DSPS24/blob/main/399_(40.7199438333333%2C%20-89.42___4166)_%202023-10-18%2015-43-34_55.86445_D.jpg" width="20%"/>
    </a>
</div> 

## <summary>TIMELINE </summary>
* 12-11-2023: Team registration begins! Challenge GitHub page and Website opens.
* 12-20-2023: Training data for competition is released. Download data from GitHub page
* 01-08-2024: Test Data for competition is released.
* 01-22-2024: Leaderboard website is open for results submission.
* 01-29-2024: Tutorial on how to use benchmark model.
* 02-12-2024: The link for submitting the source code enabled.
* 02-19-2024: Competition ends! Deadline for submitting the source code & the solutions.
* 02-22-2024: Top 5 teams shortlisted for paper submission!
* 03-11-2024: Symposium begins!

## <summary> RULES </summary>
We expect you to respect the spirit of the competition and do not cheat.
* There is no restriction on the size of the team.
* The use of external data is forbidden
* Pre-trained models are allowed in the competition
* Teams are free to use any model architecture of their choice. 
* Please submit source code and trained model before the deadline. IPython Notebook is desirable for the source code submission. The organizers will verify the reproducibility of the algorithm before determining the final winner.


# Data Download
```bash
## use gdown in google collab to download training data. 
!gdown --id '1epfGqAgjFsxNN3uFLo9GI3eI7m1yX4Jh'
```

## Data Extraction 
```bash
## use unzip in google collab to extract zipped training data to current directory. 
!unzip 'data.zip' -d './'
```
