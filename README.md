# 💴 Counterfeit Banknote Detection

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white)
![Accuracy](https://img.shields.io/badge/Accuracy-98.24%25-brightgreen)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

## Objective

Build an algorithm to **automatically detect counterfeit banknotes** based on geometric measurements, for the French OCRFM (Office Central pour la Repression du Faux Monnayage).

For each banknote, the model outputs a probability of authenticity. If >= 0.5 the banknote is genuine, otherwise counterfeit.

---

## Dataset

6 geometric features per banknote: `length`, `height_left`, `height_right`, `margin_up`, `margin_low`, `diagonal` (all in mm).

---

## Methodology

1. **Descriptive analysis** - univariate and bivariate statistics, pairplot, boxplots
2. 2. **PCA** - scree plot, correlation circle, factorial plane, `is_genuine` as illustrative variable
   3. 3. **K-Means clustering** - 2 clusters, comparison with true labels, confusion matrix
      4. 4. **Logistic Regression** - binary classifier with probability output, confusion matrix
        
         5. ---
        
         6. ## Results
        
         7. | Model | Accuracy |
         8. |-------|----------|
         9. | K-Means | ~96% |
         10. | **Logistic Regression** | **98.24%** |
        
         11. Only 3 misclassifications out of 170 banknotes.
        
         12. ---
        
         13. ## Files
        
         14. | File | Description |
         15. |------|-------------|
         16. | `HOUSSAIN_TAHIRI_P6.ipynb` | Full analysis notebook |
         17. | `dataset_Faux_Billet_Test_Exam.csv` | Training dataset |
         18. | `reg_matrice-confusion.png` | Logistic Regression confusion matrix |
         19. | `kmeans_matrice-confusion.png` | K-Means confusion matrix |
         20. | `acp_isgenuine.png` | PCA factorial plane by authenticity |
         21. | `cercle-correlations.png` | PCA correlation circle |
         22. | `kmeans-clusters.png` | K-Means clusters in PCA plane |
         23. | `pairplot.png` | Bivariate analysis |
         24. | `boxplots.png` | Feature distributions by class |
        
         25. ---
        
         26. ## Tools
        
         27. `Python` - `Pandas` - `NumPy` - `Scikit-learn` - `Matplotlib` - `Seaborn`
        
         28. ---
        
         29. ## Author
        
         30. **Houssain TAHIRI** - Data Analyst
         31. [![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/houssain-tahiri-246b00100/)
