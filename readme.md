### 1. Title
Predicting whether and when a betrayal will occur based on linguistic features
### 2. Abstract:
The original article addresses two questions. The first question is to predict whether a betrayal will occur, and the second is to predict when betrayal is going to occur knowing the fact that the betrayal is doomed to happen.   
We think that the second question is unrealistic, because it is impossible to know whether betrayal will occur in reality. A more important and more practical question is: given a dialogue, can we predict whether a betrayal will occur, and at the same time predict when the betrayal will occur (if we predict it will). The motivation for our work is exactly to address this question.

### 3. Research Questions
While playing the game Diplomacy or in real life, knowing that we are going to be betrayed is not enough, we would also like to know how far betrayal is near us if we know such betrayal is going to happen. We will focus on such a question: Without knowing if a betrayal will occur, predict if there will be a betrayal and if it will, predict when it is going to happen.

### 4. Proposed Dataset
We will use the same dataset as the original paper, and on its bases we will make a few pre-processings.

### 5. Methods Description

**Replicating the models in the paper:** We will first replicate the two models described in the original paper (Namely, we build a first model to predict if there will be a betrayal, and the second model to predict when the betrayal will happen.). However, we will make a few changes and improvements on them. First: The models in the paper consider seasons as classification instances, we think such assumptions are not practical, so we treat games as classfication instead. Besides, when predicting which season is the betrayal season in a game, we make sure that only one season in each game would be predicted to be the season in which betrayal happened. 

**Connecting the models to generate final result:** Another improvement we will make on the papers is that, the two models we built will not be independent from each other (like in the paper). We would make a link between the two models and combine their results to make our final prediction: namely predict whether a game would end up in betrayal, and if yes, when the betrayal would happen. 


### 6. Proposed Timeline
In the first week, we will replicate the training of the two models in the original paper.

In the second week, we will make our changes and improvements on the basis of the models in the paper.

In the third week, we will make a link between the two models, analyze the results and write our final report.

### 7. Organization within the team
In week 1, Shanci will replicate the first model in original paper, and Ke and Ruizhi will replicate the second one.

In week 2, we will respectively make the changes and improvements to the models which we are responsible of. 

In week 3, Ke and Ruizhi will make the link between the models and combine their results, then all of us write our final report together.
