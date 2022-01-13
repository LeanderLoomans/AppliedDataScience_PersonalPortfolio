# Applied Data Science: Personal Portfolio
Name: Leander Loomans <br />
Studentnumber: 21136769 <br />
Course: Applied Data Science Minor <br />
Teachers: Jeroen Vuurens, Tony Andrioli, Ruud Vermeij <br />


## DataCamp Course

<details><summary>Show Content</summary>

Overall, the DataCamp courses proved to be very useful. They accompanied the lectures by Jeroen and Tony nicely, and provided a way to bring into practice what you were taught, even if your project was not yet ready for writing code. Then, when the project entered the coding phase, it felt as if I had a head start, because I had already fooled around with lots of the machine learning functions. I have completed 100% of the courses, as can be seen below.

<details><summary>DataCamp Completion</summary>
  
![Image 1](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/images/DataCamp0.png)
  
![Image 2](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/images/DataCamp1.png)
  
</details>

It should be noted that I was familliar with Python before starting this minor, as it was taught during one of the classes in the first year of my major Software Engineering.

</details>
  
## Reflection and Evaluation

<details><summary>Reflection on Own Contribution to the Project</summary>

#### Situation
At the beginning of the minor, I chose to be part of the Dialogue team, along with 5 other students. I chose this project, because the detection of social interaction seemed like an incredibly interesting and versatile subject, that could also be deployed in many other situations than just in the context of the Smart Teddy project. I never regretted my decision for a second, also because I had a great group to work with. I thought the lectures by Jeroen and Tony were very useful and always relevant to our current objectives in the project. We used Scrum with two week sprints and daily stand-ups to guide our process to the right direction, which was always a nice support to have. 

#### Task
The first few weeks we divided ourselves into groups with different objectives. Me and Olaf had to get familiar with machine learning algorithms and the processing of sound in a way that a model could learn information from it. These first step laid a great base for the rest of our work. I ended up becoming the ‘expert’ on the dataprocessing aspect of the project, but cooperated a lot with Olaf on this. Vice versa, his specialty was configuring our neural networks, but while cooperating I got to give a lot of input there as well. At the end of the project, the whole group became more focussed on the research paper, so that also became my main focus. 

#### Action
For the dataset provision for the neural networks, I started by looking for existing datasets. The way I researched this, besides just searching on Google and Kaggle, was to look into the research that described similar projects to our own, and see what datasets they used. Next, I had to process this data into something that the network could easily understand. This was initially spectrograms, but later I decided to try using MFCCs instead. This made our accuracy score jump up quite a bit, around 10%, so we were all very happy with that decision. 
At one point we also switched from using generated images to using the raw MFCC data, following critical questions during one of the external presentations. We used images because we had initially misunderstood what Jeroen and Tony tried to explain to us, and I had had my doubts about this ‘back and forth’ translating of the data, but didn’t share this with the group because we did get promising results from the networks. I later regretted not sharing my thoughts, because then we might have gotten better results earlier.

#### Result
The results of my work are Jupyter Notebooks which generate datasets from audio, to train our two neural networks with and to test our final product on. I am pleased with these generator-algorithms. They are written to be very flexible and can be adjusted to produce different kinds of datasets, often by adjusting just a couple of global variables or changing out a single line of code. I also optimized my dataset generators to be as fast as I could get them. An example of this is The [Speaker Combi Generator](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/code/SpeakerCombiGeneratorEnhanced.ipynb), which first took hours to run, and after optimization only took seconds. This enabled us to switch back and forth rapidly between generating and training, allowing us to make quick adjustments and learn about what worked and what didn’t. I tried to put in comments to clarify the inner workings for the others, but I could definitely have documented my code better, so that’s something I want to improve in the future.

#### Reflection
I think I was able to provide a valuable contribution to my team. Overall, I was very active in the devising and discussing of ideas, making plans, dividing tasks and working on our results. As mentioned above, there are some things I would like to improve myself in. If I have doubts, I shouldn’t keep them for myself. Also, I should keep others more informed of my work. I think my team always knew what I was working on, in part thanks to the scrum board. But I doubt anyone else can describe in detail how the dataset generators work. On the other hand, software engineering wasn’t really part of the learning objectives of this minor anyway. Something I think I did do well, was providing a positive mental attitude in the group. I always actively tried to keep the mood up and diffusing tense situations with a joke. I was always able to get the rest to go along with it, so we ended up having a great time during this minor.
  
</details>

<details><summary>Reflection on Own Learning Objectives</summary>
  
#### Situation
What I wanted out of this minor, primarily, was to learn how to make predictive models. I had no prior knowledge or experience with machine learning, and hardly any experience with data science as a whole. The only experience I had was plotting some graphs in python in my first year of Software Engineering. However, I was aware of the possibilities of machine learning. I had seen what is possible on the news and on the internet, and I liked that so much that I wanted to be able to do all those awesome things for myself. 

#### Task
At the beginning of the minor I set some goals for myself. I made a list of what I wanted to learn over the course of this minor. First of all, I wanted to learn how to create functioning machine learning models. Second, I wanted to learn how to select and process data for these models to train on. Third, I wanted to gain experience in performing a good research and writing a paper. Fourth and finally, I wanted to gain experience in working for a project that was bigger than my study. 

#### Action
The way I wanted to achieve my first and second learning objectives, was by taking tasks upon myself that involved me in writing code. I did this by assigning my name to those tasks on the scrum board. My third learning objective, I worked on by studying lots of other research that was about similar projects to our own. This, together with the workshop by Tony and feedback from him and Jeroen, taught me a lot. For my fourth learning objective I tried my best to be proactive during the meetings with Hani, our problem owner. I often proposed to my team to prepare together for the meeting by writing down all the questions that we had, and topics that we wanted to discuss with him. This helped us a lot in the way we presented our selves from a professional point of view.

#### Result
I created a couple of machine learning models myself: in the first few weeks I made a model that was able to, to a certain degree, predict which character said a quote in South Park. Later, during the hackathon, I created a random forest classifier which had the best results of our group, and would have been the second best of the whole class if I had gotten around to using the right dataset to test on. Furthermore, I even have a good grasp of how neural networks function and how to create/tweak them, from working together with Olaf on our convolutional neural networks. For my last learning objective, at the time of writing this evaluation we haven’t given our final presentation for Hani yet so I have no feedback from him as result. However, the result that I do have is that I experienced how motivating it is to work on something bigger than yourself. Because of that motivation, I pushed myself to perform better than just aiming for a passing grade, because our project actually matters. This was a very nice feeling to have while working on the project. 

#### Reflection
Having improved in all my learning objectives, I feel very good about my progress in this project. Not only did I learn new skills about the set objectives, there were also fields I gained knowledge in that I could not have foreseen, like how audiodata is stored or what an MFCC is and how they are made, which I am very pleased with. Now that I know how much more there is to learn, I really want to continue improving myself in the field of machine learning after this minor.

</details>

<details><summary>Evaluation on the Group Project as a Whole</summary>
  
#### Situation
My fellow students have many different backgrounds and skillsets. From the first day there were great vibes in the team. Since Björn is from Sweden, we spoke English most of the time. This didn’t bother anyone. If anything it made things a bit easier, since most of the terminology of the subject matter was in English anyway. Everyone was motivated to deliver a good result and was prepared to put in the work for it. I always felt like I could trust people to keep their word. Honestly, I could not have asked for a better team.

#### Task
One of the things we had to figure out in this team, was how to make use of everyone’s unique skills. For the software engineers this was pretty straightforward, but for the others, we had to figure it out as we went along, which we certainly did. To give an example, Olaf’s major is electrical engineering. But we were able to greatly benefit from his knowledge, because he had experience with analyzing and processing audio signals. He was able to explain to us what we needed to know, so the rest of us could get started. Likewise, everyone was able to bring a unique value to the table.

#### Action
The way we kept our group project organized, was with the help of scrum. We used a scrum board to keep track of what everyone was working on, and held daily stand-ups to share what we learned or ask for advise on how to move forward. Also, to keep everyone on the same page with regard to our views on the bigger picture of course. Finally, to give each other feedback on the process and our functioning as a team in general, we held a retrospective at the end of each sprint. These were always useful, and everyone participated seriously. We had a rule that you have to say at least one point of improvement because otherwise someone might feel awkward critiquing somebody they hardly know. This worked very well. Feedback was always given respectfully and received with dignity, as should be the case in a healthy work environment.

#### Result
I have participated in many group projects during my study, and I have to say things rarely go as smoothly as they did within our group. Communication was great, there were no heavy discussions, or in fact any negative energy in the group at all. Also, everyone was very motivated to finish their tasks, and to help others finish theirs. Without having received any results from our paper or individual test scores, I would say everybody also got to work on their learning objectives. All of us working until late in the evening on our research paper, giving feedback on each other’s writing and proof reading over and over again was another example of our great team spirit.

#### Reflection
Participating in Team Dialogue was a great experience. There was a good balance between being productive and getting things done, bonding over lunch, exchanging cultural differences and similarities with our pet Swede, and the mandatory things like (bi-)weekly meetings, lectures and workshops. Our amazing results are definitely derivative from our positive mental attitude and collective motivation. We are even going to try to get our paper published, which would be out of the question had everyone not put so much effort into it.
  
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
  
![Image 3](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/images/confusion_matrix_voice_detection.png)
  
![Image 4](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/images/confusion_matrix_voice_comparison.png)
  
</details>

When the two models are combined into the final product, the accuracies for the first and the second model are 0.88 and 0.85 respectively. With these results, we can give an answer to our research question, "How can data science techniques detect if there is a conversation between at least two people by analyzing audio files?". We got our results by training two CNNs, using one MFCC per 0.5 second of audio as input. For the final product, the audio to be analyzed is first split into 0.5 second fragments. Then, each fragment is converted to an MFCC. These are given to the first model to determine if there is speech present. If yes, it is passed on to the next model and compared to the previous MFCC. The second model then decides if the two MFCCs are by the same or a different speaker. This way the program will always work, no matter how many speakers there are, since it was never trained on a specific amount if unique speakers. With the outputs from the two models, the chances of a conversation present can be estimated.

  
### Planning
At the beginning of the minor, we decided to use SCRUM for our planning. A sprint lasted 2 weeks, with daily stand-ups and a retrospective at the end. We put our planning on a scrum board on Taiga at the beginning of each sprint. This was done by the scrum master. We decided that everyone had to have some experience with planning, so each week someone else got to play the role of scrum master. It was my turn during the second sprint. I added the user stories to the scrum board and to each user story, a certain amount of points were assigned based on the amount of time it would take to complete. This allowed us to view our progress in the burn chart at the top of the board, and compare it to the ‘ideal completion rate’ baseline. Finally, the user stories were divided up into individual tasks that could be assigned to the group members. Everyone was responsible to keep their own tasks up to date, so that the rest of the group knew what everyone else was doing and what their progress status was. How the scrum board looked at the end of the sprint can be seen in the figures below.
  
<details><summary>Scrum Board Sprint 2</summary>

Example of the scrum board of sprint 2
![Image 5](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/images/Scrumboard.png)
  
Example of an unfolded user story
![Image 6](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/images/Scrumboard_Userstory.png)
  
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
I found the three datasets that we ended up using by either searching on Google and Kaggle using keywords like ‘speech recognition’, ‘home environment’ or ‘voice activity’, or by following references to datasets in other research, similar to ours. In the case of AVA and CHIME-Home, the datasets were documented in their own papers. I used this to base my informative summaries on, which were used in our own research paper. These summaries are highlighted in the excerpt from our paper below. <br />

<details><summary>Data Summaries in Paper</summary>
  
![Image 7](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/images/DataInfo.png)
  
</details>

The LibriSpeech dataset, we needed analyze ourselves. For the script that generates datasets for the second model, it was important that the code never tries to exceed the number of speakers or the amount of files that a speaker has. For this purpose, I made the following visualization. <br />
  
<details><summary>Data Visualization LibriSpeech</summary>
  
![Image 7](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/images/Distribution_LibriSpeech.png)
  
</details>

### Data Cleansing
For creating the testing audio for our final product, we needed speaker audio with the speaker ID as label, mixed with non-speaker audio of a household environment. The most suitable dataset we could find was called 'CHIME-Home', which contained speech and non-speech audio fragments. However, we could not use the speech fragments, since they were not labeled with who was speaking (only if it was an adult male, adult female or child) and there was not enough variation in the speech. I then decided to use the LibriSpeech dataset (which we had already found) for speech audio, and only use the non-speech audio from CHIME-Home. This meant I had to filter out all files containing speech from the dataset, which turned out to be more difficult than expected: instead of having been sorted into folders by label, or containing the label in the filename, each file has a unique string of numbers, for which the corresponding labels were described in a CSV file (one CSV per audiofragment!). So, in order to clean this dataset, I had to write a custom python script that read every audio file, opened the corresponding CSV file, read the label inside it and copy the audiofile to a corresponding labeled folder. This resulted in a folder with only audiofiles containing environmental noises and no speech, which was exactly what we needed. To verify that the data we separated was the correct audio, besides listening to the audio, I checked if the ratio between voice and non-voice audio corresponded with the ratio of labels described in the CHIME-Home documentation, which it did.

[The script can be found here](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/code/Chime-Home%20Dataset%20Separator.ipynb)

### Data Preparation
The dataset for our second model has to predict whether two speech audio fragments are by the same speaker or by a different speaker. I wrote a script that generates a custom dataset based on the LibriSpeech dataset. The audio files from this set are all in one folder, and have the speaker ID in the filename. The script first allows the user to set two parameters: the amount of different speakers you want to include in the dataset (with a maximum of 251, which is the amount of speaker IDs in the dataset), and how many combinations you want to generate for each speaker. For example, when this is set to 10 combinations, the script will generate 10 combination samples where one speaker is paired with themselves, plus 10 combinations where the speaker is paired with random samples by 10 other speakers. The script separates the audio into 0.5 second fragments: the interval we chose for the model to analyze. This audio fragment is resampled to 44.1kHz to ensure homogeneity over all audio used. It then creates an MFCC of 40x44 for each audio fragment. The script also keeps track of what the labels should be: <i>true</i> for combinations from the same speaker and <i>false</i> for combinations by different speakers. The output is three .npy files: a list of MFCCs by the first audio fragment of the combinations, the MFCCs of the second fragment in the combination, and a list of all corresponding labels. 

[The script can be found here](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/code/SpeakerCombiGeneratorEnhanced.ipynb)

### Data Explanation
For our research paper, we needed to describe all of the datasets that our models use: AVA-Speech, CHIME-Home and LibriSpeech. I wrote these sections in the ‘Dataset’ and ‘Testing Datasets’ subsections in Methods. These bullet point descriptions (and TABLE I) serve as a quick overview for readers to see what we look for in a dataset for this project, as well as ensuring that, should our research be repeated, the same datasets are used in the same composition we did.


### Data Visualization
A good eample of data visualization is a script I wrote about the AVA-Speech dataset. The code uses the same methods to create MFCCs per 0.5 second of resampled audio, as was used in every code to make the datasets. A random MFCC is visualized, along with a generated pie-chart showing the ratios between labels: ‘NO_SPEECH, CLEAN_SPEECH, SPEECH_WITH_NOISE, SPEECH_WITH_MUSIC’. These visualizations proved to be very useful for verification that the process went right, balancing the datasets in our favour, and to tailor the first layer of each of the networks to accept the input shape (40x44) without error.

[The script can be found here](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/code/DataVisualisation.ipynb)

</details>

## Communication

<details><summary>Show Content</summary>

### Presentations
I prepared and presented for internal presentations on [20/09/2021](https://docs.google.com/presentation/d/1_keYMeNEbK_fAQeNPD3XL43IEjjmxnUrA34O2uwElBM/edit?usp=sharing), [11/10/2021](https://docs.google.com/presentation/d/1kMJasKvAMTAsOC0VdpSAt23xNqxIQ201jdoMdJYYSj8/edit?usp=sharing) and [22/11/2021](https://docs.google.com/presentation/d/1CkHC8wt1oXxLab80V8DGILgZA2loFwMduMZKvBJb8Zg/edit#slide=id.p). This was always together with one other group member, except for the first presentation, which we did with the whole group. I also helped prepare and give the external presentation on [08/10/2021](https://docs.google.com/presentation/d/1WzA2z_zZoB8E06DbU7IOXA3dTB0pueHfBE-lGYLRYFo/edit#slide=id.g6c52a2e8d8_0_177).

### Writing Paper
I started contributing a bit later on the research paper than some of my other group members. There was a moment, a week before Christmas, where we decided to stop trying to improve our product and we all should focus on the paper. Up until then I had only weighed in on the decision making. When I started writing, there was already a clearly defined structure for the document. However, once I did start writing, I wrote a lot of the text in the final version. I wrote the <i>Dataset</i>, <i>Testing Dataset</i>, <i>Data Preparation</i> and <i>Neural Networks</i> sections in <i>Methods</i>. I also wrote the second paragraph of <i>Results</i>, and the last three paragraphs of <i>Recommendation</i>. This comes down to 975 words, which is 23% of the total of 4212 words. This is more than the 1/6 average, since everyone from Team Dialogue participated in writing the paper. <br />
Besides writing, I also gave detailed feedback to all other sections in the paper multiple times, and often joined in on discussions and decision making moments countless other times. In conclusion, I contributed above average to the final version of the paper. However, since some of my group members had started on the paper structure way before the rest joined, they have spent more time on it than I have in total.

[The entire paper can be found here](https://github.com/LeanderLoomans/AppliedDataScience_PersonalPortfolio/blob/main/docs/AppliedDataScience_Paper_V1.pdf)

</details>
