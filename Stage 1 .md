# **STAGE 1 MACHINE LEARNING AND DATA SCIENCE TASK**

(@Hackbio @slack @Charlotte @ChaimaBenMohamed @igwebuikevee0000 @Bonita)

## **Introduction**

The article Multi-omic machine learning predictor of breast cancer therapy response by Sammut et al., 2022 presents a novel approach to predicting breast cancer treatment outcomes using machine learning and multi-omic data integration. Breast cancer is a heterogeneous disease where tumor characteristics, including genetic mutations and immune response, play a crucial role in determining therapy effectiveness. To address this complexity, the researchers enrolled 168 breast cancer patients treated with chemotherapy, with some also receiving HER2-targeted therapy. They analyzed pre-treatment biopsies, focusing on tumor mutation burden, immune infiltration, and other factors to assess their correlation with therapy outcomes like pathological complete response (pCR) or residual disease.

## **Machine learning model architecture and performance**

The core focus of the article is the machine learning framework developed to integrate these diverse data types into a predictive model for breast cancer treatment outcomes. The machine learning pipeline involved key preprocessing steps, including one-hot encoding and feature selection through univariable selection and collinearity reduction. The ensemble model combined predictions from logistic regression, support vector machines (SVM), and random forests (RF), using five-fold cross-validation to optimize hyperparameters and prevent overfitting. This multi-omic data integration approach significantly outperformed using clinical variables alone, achieving an area under the curve (AUC) score of 0.87 in external validation, proving the effectiveness of the model in predicting therapy response.

## **Biological findings**

The findings revealed that pre-treatment tumor characteristics, such as immune activity and mutation profiles, are key factors influencing treatment outcomes. Tumors with high mutation burdens and immune activation were more likely to respond favorably to therapy, particularly in HER2-negative cancers. Furthermore, the study emphasized the role of clonal diversity and subclonal mutations in treatment resistance, identifying these features as critical for understanding residual disease.

## **Conclusion**

This work underscores the power of multi-omic data integration in machine learning models, demonstrating how complex biological characteristics can guide personalized medicine. By using comprehensive multi-omic datasets, the study enhances therapy response predictions, providing a foundation for more tailored, effective breast cancer treatments. This approach offers promising avenues for improving treatment for chemoresistant tumors by suggesting novel therapies when conventional treatments may not be effective.

## **REFERENCES**

Sammut, S. J., Crispin-Ortuzar, M., Chin, S. F., Provenzano, E., Bardwell, H. A., Ma, W., Cope, W., Dariush, A., Dawson, S. J., Abraham, J. E., Dunn, J., Hiller, L., Thomas, J., Cameron, D. A., Bartlett, J. M. S., Hayward, L., Pharoah, P. D., Markowetz, F., Rueda, O. M., Earl, H. M., … Caldas, C. (2022). Multi-omic machine learning predictor of breast cancer therapy response. Nature, 601(7894), 623–629. https\://doi.org/10.1038/s41586-021-04278-5
