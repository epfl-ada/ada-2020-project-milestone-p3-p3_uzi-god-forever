### 1.Title
Simultaneously Predicting If And When A Betrayal Will Occur

### 2.Abstract:
The original article addresses two questions. The first question is to predict whether a betrayal will occur, and the second is to predict when betrayal is going to occur knowing the fact that the betrayal is doomed to happen. We think that the second question is unrealistic, because it is impossible to know whether betrayal will occur in reality. A more important and more practical question is: given a dialogue, can we predict whether a betrayal will occur, and at the same time predict when the betrayal will occur (if we predict it will). The motivation for our work is exactly to address this question, and adopt two different methods to address it, and record the their performance on this question.

### 3. Research Questions
As described in our abstract, we will focus on such a question: Without knowing if a betrayal will occur, predict if there will be a betrayal and if it will, predict when it is going to happen.

### 4. Proposed Dataset
We will use the same dataset as the original paper.

### 5.Methods
#### 5.1 Methods description
To address this question, we will use two different methods.

Replicating the models in the paper and connecting them: The first one is we will connect the two models in the original paper. Namely, we will first use the first model in the paper to predict if there will be a betrayal, and if it is predicted to be true, we will hand over the data to the second model to predict when the betrayal will happen.

Building a new regression model: About the second model, we will construct a regression model, which simultaneously predict if and when a betrayal is going to happen. To achieve this, we may introduce a threshold, and if the number of seasons before the betrayal is larger than the threshold, we consider the betrayal will not happen (just a temporary idea, will be improved later).
#### 5.2 Motivation for adopting the second method
The problem with using the models in the original paper to address this question is, the second model (the model to predict when the betrayal occurs knowing it will) in the paper is trained with all betrayal data. So if it is fed with the data of non-betrayal, it will perform badly because it has never seen such data during training. So we want to combine the two models to a single model, and train it with both betrayal and non-betrayal data, so even if it miss-predicts the non-betrayal data to be betrayal, it can still predict the data to be very unlikely to betray, which means that the betray won’t happen very soon. 

### 6. Proposed Timeline
In the first week, we will replicate the training of the two models in the original paper and connect them to address the question in 3.
In the second week, we will train our proposed model to address the question in 3 and we will compare the results by the two different approaches and analyze the results.
In the third week, we might still do some analysis that if our proposed model have some improvements. Then we will prepare for the video and the report.

### 7. Organization within the team
In week 1, Shanci will replicate the first model in original paper, and Ke and Ruizhi will replicate the second one.
In week 2, Ke and Ruizhi will complete the construction of our proposed model. Then all us will compare and analyze the results of two methods. 
In week 3, Ke and Shanci will focus on preparing the short video with main ideas. Ruizhi and Shanci will make some visualizations which will be used in video and data story.
