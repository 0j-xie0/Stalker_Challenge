# Stalker Challenge for Data Scientists
•Assume a “stalker” is someone who, in this dataset, visits some of the same locations as another person, after the other person goes to that location.  
•A “stalker score” for a pair of people, A & B, is the number of locations for which A has visited a location followed by B visiting that same location in the future.  
•Any given location should be counted once in the score, so a stalker score can never be higher than the number of unique locations that A and B have in common.  
1. Which friend pair has the highest “stalker score”?  
2. Which non-friend pair has the highest “stalker score”?  
Please give the winning user id pairs and “stalker score” for each question, and please explain your solution methods, including any source code if you wrote any.

# Installation
•Clone this repo to your computer.  
•Download the dataset I have cleaned [here](https://www.dropbox.com/s/3gkszy08mfoq43q/Stalk_Cleanest_v3.pickle?dl=0)  
•OPTIONAL: original dataset is available [here](https://snap.stanford.edu/data/loc-gowalla.html)  
•Install the requirements using pip install -r requirements.txt.  
•Make sure you use Python 3.  
•You may want to install [Jupyter](http://jupyter.org/install) to run the ipynb.

# Usage
•Run the Jupyter Notebook "Stalker.Work.ipynb" either in Jupyter or the IDE of your choice.

# Tasks Performed
•Cleaned original dataset, converted to Pandas dataframe and exported to Pickle archive.  
•Filtered data by:  
••sorting according to specific columns.  
••creating separate columns.  
••dropping columns.  
••selecting specific values.  
••selecting duplicate values.  
••creating separate dataframes.  
••combining dataframes.  
••intelligent query and analysis.

# Observations
•User IDs 40090 & 132961 are clearly the highest scoring Friend-Pair based on the frequency of their meetings (181 times) and their arrival time (9.834 seconds apart) at the same location.  
•User IDs 18813 & 107599 are the winning Non-Friend-Pair based on the frequency (76 times) of arriving at the same location 409.868 seconds (6.831 minutes) apart, which is plausible because a stalker would arrive a few minutes later (but not too much later, I set the range to be 3-7 minutes apart) so as not to arouse suspicion.


