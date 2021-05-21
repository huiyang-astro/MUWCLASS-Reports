This folder contains Cross-Validation results of the training datasets. 

We test the classification accuracy by applying the Leave-One-Out Cross-Validation (LOOCV), which is a special case of cross-validation where every source in the TD will erase its label (actual source class) and be classified after training the classifier using the remaining sources in the TD. The outcome of this procedure is summarized by the Confusion Matrix where each row represents the fraction of sources in a predicted class while each column provides the fraction in an actual class. A more diagonal matrix represents a better performance. 

The different confusion matrices below are built on 
1) different selections of features, including all possible features, specifically from extensive combinations of colors, and a selection of important features with their feature importance above 1% (see the feature importance plots at the very bottom)
2) different numbers of MCMC simulations to be averaged (for testing of convergence)
3) different averaging method: i. average CM method
   * dd
   * 
4) dwd  


Description   |      Confusion Matrices (CM)   | Receiver operating characteristic (ROC) Curves| 
:------------:|:-------------------------:|:-------------------------:|
All (including 2 random) features, 11 simulations, average CM method  |![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_allfeatures_11ave_CM.png)  |  ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_allfeatures_11ave_ROC.png)
All (including 2 random) features, 11 simulations, average CM method, over 70% confidence  |![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_allfeatures_11ave_70CM.png)  |  ![]()
All (including 2 random) features, 11 simulations, average probability vectors method  |![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_allfeatures_11Probave_CM.png)  |  ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_allfeatures_11Probave_ROC.png)
Selected features, 100 simulations, average CM method  |![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100ave_CM.png)  |  ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100ave_ROC.png)
Selected features, 100 simulations, average CM method, over 70% confidence  |![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100ave_70CM.png)  |  ![]()
Selected features, 100 simulations, average probability vectors method  |![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_no_Conf_CM.png)  |  ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_no_Conf_ROC.png)
Selected features, 100 simulations, average probability vectors method, sigma Confident   |![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_sigma_Conf_CM.png)  |  ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_sigma_Conf_ROC.png)
Selected features, 100 simulations, average probability vectors method, 70 Confident  |![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_70_Conf_CM.png)  |  ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_70_Conf_ROC.png)
Selected features, 100 simulations, average probability vectors method, both Confident   |![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_both_Conf_CM.png)  |  ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_both_Conf_ROC.png)



Description   |     All (including 2 random) features, 11 simulations, average CM method  | All (including 2 random) features, 11 simulations, average CM method, over 70% confidence | All (including 2 random) features, 11 simulations, average probability vectors method | Selected features, 100 simulations, average CM method  | Selected features, 100 simulations, average CM method, over 70% confidence  | Selected features, 100 simulations, average probability vectors method  |Selected features, 100 simulations, average probability vectors method, sigma Confident   | Selected features, 100 simulations, average probability vectors method, 70 Confident  |Selected features, 100 simulations, average probability vectors method, both Confident   |
:------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|
Confusion Matrices (CM) | <img src="https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_allfeatures_11ave_CM.png" alt="drawing" style="width:200px;"/>  | ![drawing](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_allfeatures_11ave_70CM.png) | ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_allfeatures_11Probave_CM.png)  | ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100ave_CM.png)  | ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100ave_70CM.png)  |   ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_no_Conf_CM.png)  | ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_sigma_Conf_CM.png)  | ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_70_Conf_CM.png) | ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_both_Conf_CM.png)  
Receiver operating characteristic (ROC) Curves| ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_allfeatures_11ave_ROC.png) | ![]()|  ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_allfeatures_11Probave_ROC.png) | ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100ave_ROC.png) | ![]() | ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_no_Conf_ROC.png) | ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_sigma_Conf_ROC.png) | ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_70_Conf_ROC.png) |  ![](https://github.com/huiyang-astro/MUWCLASS-Reports/blob/main/Evaluations/L1O_selfeatures_100Probave_both_Conf_ROC.png)



 
 
 

