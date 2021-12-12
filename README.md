# Classification Model Application to Soccer Matches

## Introduction
The purpose of this project was to see if machine learning models could correctly classify the outcome of a match between two teams based on their attributes. I personally have been a fan of soccer or what most other non-American countries would call 'football', for a good portion of my life. My grandparents being immigrants from Eastern Europe often had me up early watching matches on the TV or even up late watching recordings on VHS. I am also very interested in Data Science and my journey in college has lead me to have a Data Science minor. So combining two things that I love working with seemed like a good project to take on. 

## Selection of Data
The reason I selected the data is because I believe it is the most baseline, logical determiner of outcome between two teams, who's stats are better. I know there is tons of other factors such as home field advantage, injuries, "throw-away games", match-up history etc. but the most reliable and easily calculable is the cold, hard stats. Another thing I would like to mention about my specific approach to the data is that I took a very heavy ignore approach to missing data in order to try and keep a accurate and consistent feature structure that my model would be using, I ended up dropping certain samples if their data wasn't at least partially complete through all three data sets. There is instances however where a team would have one or two stats which were completely missing, in that case I would fill it with the most frequent value that appeared in that column in order to save the number of samples I had.

## Methods
The methods I used were pandas and numpy in the construction and management of the data in dataframes. The preprocessing is mostly sklearn with a touch of pandas. The applied models were all Naive Bayes, which I implemented through sklearn. Lastly, the visualizations were created using a mix of matplotlib and seaborn.

## Conclusion
My most important findings, while I don't have a ton of experience in models and their intricacies, were that with the models I was able to feasibly deploy, the accuracy is approximately 50% for being able to correctly match the outcome of a match. Due to the nature of sports and their lack of uniformity, 50% is, in my opinion, a very acceptible accuracy. On the more accurate models I noticed a pattern where the models were able to most accurately predict wins, least accurately predict draws and mildly accurately predict losses. The only conclusion I could draw from this is that the binary of winning or losing is easier to identify when using numbers and encoded categorical data than the result of a draw because, in my human-mind, I would believe bigger numbers equals win, lower numbers equal lose and if the numbers are even it would be a draw, however the range of similar numbers is very arbitrary in regards to the actual outcome of a draw. (These results are in the eyes of the "home team" as recognized in my data.)

## Discussion
The conclusion implies that the prediction of sports outcomes still require more accurate models, this matters because sports is a major stepping stone in machine learning that can bridge the gap between pure mathmatical, categorical and statistical modelling and the real world. Other models that I was able to find which were used for sports prediction achieved about a 50-60% accuracy which is only about a 10% difference between my model. If we are able to master using machine learning on something as dynamic as sports, there's no telling how far that can expand into the real world, from markets to politics to warfare, machine learning could end up becoming an accurate version of the magic eight ball.


### To whom it may concern

The information about the application is all available in the attached notebook.

The notebook was made on Google Colab so the data retrevial and some of the formatting may not work as intended.

Viewing access to my Google Colab notebook is [here](https://colab.research.google.com/drive/1CkHq6P33IE62aVJPFO67Gnj7jhNjwAj9?usp=sharing).

I'd also like to stress that this data was used for educational purposes and does not belong to me nor does the processed version of the data, the only work that is mine is the code and text in the notebook.

Note: Due to Github's max file size I couldn't upload the matches csv. Access is available through this link [here](https://drive.google.com/file/d/1SIJGF12CiSSACpLemifoTFAdmrjtocQL/view?usp=sharing).
