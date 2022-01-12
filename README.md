# Applied Data Science: Personal Portfolio
Name: Leander Loomans <br />
Studentnumber: 21136769 <br />
Course: Applied Data Science Minor <br />
Teachers: Jeroen Vuurens, Tony Andrioli, Ruud Vermeij <br />


## DataCamp Course

<details><summary>Show Content</summary>

Overall, the DataCamp courses proved to be very useful. They accompanied the lectures by Jeroen and Tony nicely, and provided a way to bring into practice what you were taught, even if your project was not yet ready for writing code. Then, when the project entered the coding phase, it felt as if I had a head start, because I had already fooled around with lots of the machine learning functions. I have completed 100% of the courses, as can be seen below.

<details><summary>DataCamp Completion</summary>
  
![DataCamp Image 0](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/images/DataCamp 0.png)
  
![DataCamp Image 1](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/images/DataCamp 1.png)
  
</details>

It should be noted that I was familliar with Python before starting this minor, as it was taught during one of the classes in the first year of my major Software Engineering.

</details>
  
## Reflection and Evaluation

<details><summary>Show Content</summary>

### Reflection on Own Contribution to the Project
At the beginning of the minor, 

### Reflection on Own Learning Objectives

### Evaluation on the Group Project as a Whole

</details>

## Research Project

<details><summary>Show Content</summary>
  
### Task Definition
I was part of Team Dialogue during this minor. Team Dialogue is part of Smart Teddy, an innovative project of The Hague University of Applied Sciences. Its goal is to apply data science to improve the quality of life of dementia patients, by enabling them to stay in their own homes for longer. The Smart Teddy is equipped with sensors, among others a microphone, to monitor the patient and their condition. Algorithms will analyze the gathered data and send the results to a dashboard, where a healthcare professional can easily make an estimation of many patients’ conditions efficiently, reducing the pressure of the volunteers and the care system. When implemented correctly, all this will enable the dementia patients to live at home for longer, thus improving their quality of life. The subjects that will be monitored include presence of emotion, eating patterns and social interaction. Team Dialogue was tasked to find a solution for the latter. Specifically, our group tried to analyze audio signals to try and detect the presence of conversations. Together we formulated our assignment into one research question: "How can data science techniques detect if there is a conversation between at least two people by analyzing audio files?"

### Evaluation
On the whole, I believe that our group did very well. None of us had much (if any) experience with machine learning, and some of us had never even coded a program. I do wish, however, that I could restart the project with my current knowledge. I feel like I could do so much more now, and work so much faster than we did in the first weeks of the project. I also still have many ideas I would have liked to try, to further improve upon what we have. Improvements such as: changing the way we load data into the model, so that we can train on much bigger datasets. Or adding a third model to our final product, that can filter out noise from radio, tv or other sources that can be mistaken for speech. We could have improved our two existing models (detecting speech and comparing speakers) further, for example by adding more unique speakers to avoid overfitting on certain voices. I would have also liked to put more work into the combination of the models. Right now, the output is a percentage of speech present (by the first model) and how often the speaker changes (by the second model). But the second model can hypothetically also be used to give an estimation of how many unique speakers are in the audio, just by writing smarter code that compares more audio fragments than just two consecutive ones. Sadly though, there just wasn’t enough time. The fact that the best ideas came later in the project only shows that I learned so much, that I made a huge improvement over the course of this minor and that I learned many new skills, so I’m certainly happy with that.

### Conclusions
The results we ultimately got on both our models are actually very impressive, especially for a group of first time data scientists. The first model (detecting speech in one MFCC) got an accuracy of 0.89, and the second model (detecting if two MFCCs are the same or different speakers) got an accuracy of 0.94. Both datasets were balanced 50/50 between <i>true</i> and <i>false</i> samples, so those scores really do mean that the models work. The chance of getting those scores with blind guesses is less than 0.000000000000013%. The confusion matrices for both models are shown below. 
  
<details><summary>Confusion Matrices</summary>
  
![DataCamp Image 3](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/images/confusion_matrix_voice_detection.png)
  
![DataCamp Image 4](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/images/confusion_matrix_voice_comparison.png)
  
</details>

When the two models are combined into the final product, the accuracies for the first and the second model are 0.88 and 0.85 respectively. With these results, we can give an answer to our research question, "How can data science techniques detect if there is a conversation between at least two people by analyzing audio files?". We got our results by training two CNNs, using one MFCC per 0.5 second of audio as input. For the final product, the audio to be analyzed is first split into 0.5 second fragments. Then, each fragment is converted to an MFCC. These are given to the first model to determine if there is speech present. If yes, it is passed on to the next model and compared to the previous MFCC. The second model then decides if the two MFCCs are by the same or a different speaker. This way the program will always work, no matter how many speakers there are, since it was never trained on a specific amount if unique speakers. With the outputs from the two models, the chances of a conversation present can be estimated.

  
### Planning
At the beginning of the minor, we decided to use SCRUM for our planning. A sprint lasted 2 weeks, with daily stand-ups and a retrospective at the end. We put our planning on a scrum board on Taiga at the beginning of each sprint. This was done by the scrum master. We decided that everyone had to have some experience with planning, so each week someone else got to play the role of scrum master. It was my turn during the second sprint. I added the user stories to the scrum board and to each user story, a certain amount of points were assigned based on the amount of time it would take to complete. This allowed us to view our progress in the burn chart at the top of the board, and compare it to the ‘ideal completion rate’ baseline. Finally, the user stories were divided up into individual tasks that could be assigned to the group members. Everyone was responsible to keep their own tasks up to date, so that the rest of the group knew what everyone else was doing and what their progress status was. How the scrum board looked at the end of the sprint can be seen in the figures below.
  
<details><summary>Scrum Board Sprint 2</summary>

Example of the scrum board of sprint 2
![DataCamp Image 5](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/images/Scrumboard.png)
  
Example of an unfolded user story
![DataCamp Image 6](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/images/Scrumboard_Userstory.png)
  
</details>
  
</details>

## Predictive Analytics

<details><summary>Show Content</summary>

### Selecting a Model

### Configuring a Model

### Training a Model

### Evaluating a Model

### Visualizing the Outcome of a Model

</details>
  
## Domain Knowledge

<details><summary>Show Content</summary>

### Introduction of the Subject Field

### Literature Research

### Explanation of Terminology, Jargon and Definitions

</details>

## Data Preprocessing

<details><summary>Show Content</summary>

### Data Exploration

### Data Cleansing
For creating the testing audio for our final product, we needed speaker audio with the speaker ID as label, mixed with non-speaker audio of a household environment. The most suitable dataset we could find was called 'CHIME-Home', which contained speech and non-speech audio fragments. However, we could not use the speech fragments, since they were not labeled with who was speaking (only if it was an adult male, adult female or child) and there was not enough variation in the speech. I then decided to use the LibriSpeech dataset (which we had already found) for speech audio, and only use the non-speech audio from CHIME-Home. This meant I had to filter out all files containing speech from the dataset, which turned out to be more difficult than expected: instead of having been sorted into folders by label, or containing the label in the filename, each file has a unique string of numbers, for which the corresponding labels were described in a CSV file (one CSV per audiofragment!). So, in order to clean this dataset, I had to write a custom python script that read every audio file, opened the corresponding CSV file, read the label inside it and copy the audiofile to a corresponding labeled folder. This resulted in a folder with only audiofiles containing environmental noises and no speech, which was exactly what we needed. To verify that the data we separated was the correct audio, besides listening to the audio, I checked if the ratio between voice and non-voice audio corresponded with the ratio of labels described in the CHIME-Home documentation, which it did.

[The script can be found here](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/code/Chime-Home%20Dataset%20Separator.ipynb)

### Data Preparation
The dataset for our second model has to predict whether two speech audio fragments are by the same speaker or by a different speaker. I wrote a script that generates a custom dataset based on the LibriSpeech dataset. The audio files from this set are all in one folder, and have the speaker ID in the filename. The script first allows the user to set two parameters: the amount of different speakers you want to include in the dataset (with a maximum of 251, which is the amount of speaker IDs in the dataset), and how many combinations you want to generate for each speaker. For example, when this is set to 10 combinations, the script will generate 10 combination samples where one speaker is paired with themselves, plus 10 combinations where the speaker is paired with random samples by 10 other speakers. The script separates the audio into 0.5 second fragments: the interval we chose for the model to analyze. This audio fragment is resampled to 44.1kHz to ensure homogeneity over all audio used. It then creates an MFCC of 40x44 for each audio fragment. The script also keeps track of what the labels should be: <i>true</i> for combinations from the same speaker and <i>false</i> for combinations by different speakers. The output is three .npy files: a list of MFCCs by the first audio fragment of the combinations, the MFCCs of the second fragment in the combination, and a list of all corresponding labels. 

[The script can be found here](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/code/SpeakerCombiGeneratorEnhanced.ipynb)

### Data Explanation
For our research paper, we needed to describe all of the datasets that our models use: AVA-Speech, CHIME-Home and LibriSpeech. I wrote these sections in the ‘Dataset’ and ‘Testing Datasets’ subsections in Methods. These bullet point descriptions (and TABLE I) serve as a quick overview for readers to see what we look for in a dataset for this project, as well as ensuring that, should our research be repeated, the same datasets are used in the same composition we did.


### Data Visualization
A good eample of data visualization is a script I wrote about the AVA-Speech dataset. The code uses the same methods to create MFCCs per 0.5 second of resampled audio, as was used in every code to make the datasets. A random MFCC is visualized, along with a generated pie-chart showing the ratios between labels: ‘NO_SPEECH, CLEAN_SPEECH, SPEECH_WITH_NOISE, SPEECH_WITH_MUSIC’.

[The script can be found here](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/code/DataVisualisation.ipynb)

</details>

## Communication

<details><summary>Show Content</summary>

### Presentations
I prepared and presented for internal presentations on 20/09/2021, 11/10/2021 and 22/11/2021. This was always together with one other group member, except for the first presentation, which we did with the whole group. I also helped prepare and give the external presentation on 08/10/2021.

### Writing Paper
I started contributing a bit later on the research paper than some of my other group members. There was a moment, a week before Christmas, where we decided to stop trying to improve our product and we all should focus on the paper. Up until then I had only weighed in on the decision making. When I started writing, there was already a clearly defined structure for the document. However, once I did start writing, I wrote a lot of the text in the final version. I wrote the <i>Dataset</i>, <i>Testing Dataset</i>, <i>Data Preparation</i> and <i>Neural Networks</i> sections in <i>Methods</i>. I also wrote the second paragraph of <i>Results</i>, and the last three paragraphs of <i>Recommendation</i>. This comes down to 975 words, which is 23% of the total of 4212 words. This is more than the 1/6 average, since everyone from Team Dialogue participated in writing the paper. <br />
Besides writing, I also gave detailed feedback to all other sections in the paper multiple times, and often joined in on discussions and decision making moments countless other times. In conclusion, I contributed above average to the final version of the paper. However, since some of my group members had started on the paper structure way before the rest joined, they have spent more time on it than I have in total.
</details>
