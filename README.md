# Applied Data Science: Personal Portfolio
### By Leander Loomans
Personal Portfolio for the minor Applied Data Science at The Hague University of Applied Sciences

## DataCamp Course
I have completed 100% of the DataCamp course, as can be seen below:

![DataCamp Image](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/images/DataCamp.png)

It should be noted that I was familliar with Python before starting this minor, as it was taught during one of the classes in the first year of my major Software Engineering.

## Reflection and Evaluation

### Reflection on Own Contribution to the Project

### Reflection on Own Learning Objectives

### Evaluation on the Group Project as a Whole


## Research Project

### Task Definition



### Evaluation

### Conclusions

### Planning


                <!-- ## Predictive Analytics

                ### Selecting a Model

                ### Configuring a Model

                ### Training a Model

                ### Evaluating a Model

                ### Visualizing the Outcome of a Model


                ## Domain Knowledge

                ### Introduction of the Subject Field

                ### Literature Research

                ### Explanation of Terminology, Jargon and Definitions -->


## Data Preprocessing

### Data Exploration

### Data Cleansing

For creating the testing audio for our final product, we needed speaker audio with the speaker ID as label, mixed with non-speaker audio of a household environment. The most suitable dataset we could find was called 'CHIME-Home', which contained speech and non-speech audio fragments. However, we could not use the speech fragments, since they were not labeled with who was speaking (only if it was an adult male, adult female or child) and there was not enough variation in the speech. I then decided to use the LibriSpeech dataset (which we had already found) for speech audio, and only use the non-speech audio from CHIME-Home. This meant I had to filter out all files containing speech from the dataset, which turned out to be more difficult than expected: instead of having been sorted into folders by label, or containing the label in the filename, each file has a unique string of numbers, for which the corresponding labels were described in a CSV file (one CSV per audiofragment!). So, in order to clean this dataset, I had to write a custom python script that read every audio file, opened the corresponding CSV file, read the label inside it and copy the audiofile to a corresponding labeled folder. This resulted in a folder with only audiofiles containing environmental noises and no speech, which was exactly what we needed. To verify that the data we separated was the correct audio, besides listening to the audio, I checked if the ratio between voice and non-voice audio corresponded with the ratio of labels described in the CHIME-Home documentation, which it did.

[The script can be found here](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/code/Chime-Home%20Dataset%20Separator.ipynb)

### Data Preparation

The dataset for our second model has to predict whether two speech audio fragments are by the same speaker or by a different speaker. I wrote a script that generates a custom dataset based on the LibriSpeech dataset. The audio files from this set are all in one folder, and have the speaker ID in the filename. The script first allows the user to set two parameters: the amount of different speakers you want to include in the dataset (with a maximum of 251, which is the amount of speaker IDs in the dataset), and how many combinations you want to generate for each speaker. For example, when this is set to 10 combinations, the script will generate 10 combination samples where one speaker is paired with themselves, plus 10 combinations where the speaker is paired with random samples by 10 other speakers. The script separates the audio into 0.5 second fragments: the interval we chose for the model to analyze. This audio fragment is resampled to 44.1kHz to ensure homogeneity over all audio used. It then creates an MFCC of 40x44 for each audio fragment. The script also keeps track of what the labels should be: True for combinations from the same speaker and False for combinations by different speakers. The output is three .npy files: a list of MFCCs by the first audio fragment of the combinations, the MFCCs of the second fragment in the combination, and a list of all corresponding labels. 

[The script can be found here](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/code/SpeakerCombiGeneratorEnhanced.ipynb)

### Data Explanation

For our research paper, we needed to describe all of the datasets that our models use: AVA-Speech, CHIME-Home and LibriSpeech. I wrote these sections in the ‘Dataset’ and ‘Testing Datasets’ subsections in Methods. These bullet point descriptions (and TABLE I) serve as a quick overview for readers to see what we look for in a dataset for this project, as well as ensuring that, should our research be repeated, the same datasets are used in the same composition we did.


### Data Visualization

A good eample of data visualization is a script I wrote about the AVA-Speech dataset. The code uses the same methods to create MFCCs per 0.5 second of resampled audio, as was used in every code to make the datasets. A random MFCC is visualized, along with a generated pie-chart showing the ratios between labels: ‘NO_SPEECH, CLEAN_SPEECH, SPEECH_WITH_NOISE, SPEECH_WITH_MUSIC’.

[The script can be found here](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/code/DataVisualisation.ipynb)


## Communication

### Presentations

I prepared and presented for internal presentations on 20/09/2021, 11/10/2021 and 22/11/2021, and did an external presentation on 08/10/2021

### Writing Paper
