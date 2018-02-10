# Python-103
Ensemble Modelling - Prudential Life Insurance Assessment

**The Challenge:** In a one-click shopping world with on-demand everything, the life insurance application process is antiquated. Customers provide extensive information to identify risk classification and eligibility, including scheduling medical exams, a process that takes an average of 30 days.

**The Result:** People are turned off. That’s why only 40% of U.S. households own individual life insurance. Prudential wants to make it quicker and less labor intensive for new and existing customers to get a quote while maintaining privacy boundaries.

**Evaluation:** Submissions are scored based on the quadratic weighted kappa, which measures the agreement between two ratings. This metric typically varies from 0 (random agreement) to 1 (complete agreement). In the event that there is less agreement between the raters than expected by chance, this metric may go below 0.

**Proposed Solution:** Combination of Neural Network and Ensemble modelling 
*	Input Layer: Binned input variables.  
*	Hidden Layer 1: 6 Decision Tree Classifiers, 6 Random Forest Classifiers, and 6 XG Boost Classifiers. 
*	Hidden Layer 2: KNN model is used the combine the outputs of the Decision Trees, another KNN model is used to combine the outputs of the Random Forest, and one more KNN model is used to combine the outputs of the XB Boost.
*	Output Layer: KNN model is used the combine the outputs of the above KNN models.
