Yuqi He
All codes and experiments:
https://github.com/Bigmichyk123/GNN_SHAP 

Week 1 & 2 (02/05/2024 – 02/18/2024):
Read the paper “Event-Aware Multimodal Mobility Nowcasting” by Wang et al. Focused mostly on the part where they experiment models.
Attempted simple, more naïve models like historical average (HA) and naïve forecast (NF). It would be almost impossible to get SHAP to work on the explanations of these models due to their naiveness. Naïve Forecast has a significantly higher accuracy than historical average in most data.
Don't think it needed more than that to summarize, the code in google doc: https://colab.research.google.com/drive/1RabAYrrCiAWYIp2qxuTvq9tDjK_jZkNq?usp=sharing 
In Github:
https://github.com/Bigmichyk123/GNN_SHAP/blob/main/Naive%20models.ipynb 
 
Week 3 & 4 (02/19/2024 – 03/03/2024):
A simple linear regression was fitted for the convenience of using shap for models. Dataset used: COVID and JONUS. I find some difference between SHAP values between the features, although they are not crazily separable. So they are significantly different, but that does not mean they are good indications for feature selection.
A small summary:
A linear regression model is fitted on the data, poi is the response, and meta_onehot are the features, except the dimension is 1x1 instead of 1x3. The consistent “1” dimension being time.

the code in google doc: https://colab.research.google.com/drive/190cqv6aJTL_DFOTbtnviO3Rro1K5agCz?usp=sharing 
In Github:
https://github.com/Bigmichyk123/GNN_SHAP/blob/main/COVID_US_LinearModel_SHAP.ipynb 
 
Week 5 & 6 (03/04/2024 – 03/17/2024): Spring break included.
Waiting on GNN work from Chuyi, some experimentation started for SHAP. The idea is to use SHAP to try improving more naïve models. This experiment was done on 04/29/2024 and the results show that if the features’ SHAP values are close enough, they appear to have no significant difference when modeling. SHAP somehow amplifies the importance of slightly more important data. The full report will be shown later.
 
Week 7 & 8 (03/18/2024 – 03/31/2024):
Continued experimentation on SHAP’s effectiveness on simple classification tasks.
Match up with Chuyi trying to explain GNN.
 
Week 9 & 10 (04/01/2024 – 04/13/2024):
Continued experimentation on SHAP’s effectiveness on simple classification tasks.
 
 
Week 11 & 12 (04/14/2024 – 04/28/2024):
Wrapped up experimentation on SHAP and start drawing some conclusions, Chuyi has the GNN done when it was 05/01/2024. But before that, we knew the way we just explain the features of GNN within the model is infeasible. We have the problem again but that will be future work for now.
A very important conclusion is that even if the experimentation turns out to have significant differences in SHAP values, we still need to examine if that is a case where we can use SHAP as an optimizing benchmark per the experiment we did on classification.
You can find the entire experiment here:
https://drive.google.com/drive/folders/1dWriBIbL0lBwwlFwszRINUxUvdM0SNXD?usp=sharing 
Or here:[link]([doc:linking-to-pages#anchor-links](https://github.com/Bigmichyk123/GNN_SHAP/tree/main/experiment))
https://github.com/Bigmichyk123/GNN_SHAP/tree/main/experiment 
Here is the link to our final report in Google doc:

https://docs.google.com/document/d/1WJu0XCpVRynIlgzbeCg0toRLBerlgSIUiRjmwOWvksM/edit?usp=sharing 

On Github:

https://github.com/Bigmichyk123/GNN_SHAP/blob/main/experiment/Final_Report.docx 
