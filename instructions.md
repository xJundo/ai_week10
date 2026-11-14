c'est un travail de groupe ou nous avons des nouvelles taches chaque semaine. Fais les taches, en étant dans la continuité des pdfs de @resources/ car on ne veut pas inventer ou faire des trucs trop difficiles par rapport aux pdfs. Pour chaque nouvelle week, il faut recopier le notebook d'avant et ajouter les nouvelles taches.
les markdowns dans les notebooks doivent etre simplistes concis et pas trop trop IA / robotique, il faut que ça paraisse étudiant.

Voici ce qu'on devait faire dans la week 10:
     Find 3 public dataset candidates and choose 1 of them. Make a table with the source, data size (number of samples and features), and license of each candidate. Write why you chose the final one.

    Example: Kaggle "Heart Disease" / 303 samples, 13 features / CC0 license / The features are clean and the data is small, so we can run many experiments.

    Define the problem you will solve with the chosen data. Write the input, the target, and the problem type (binary classification, multiclass classification, or regression).

    Example: Binary classification that predicts heart disease (target) from a patient's test results (input)

    Choose the evaluation metric that shows success and explain why. Check the class ratio. If the classes are in imbalanced, consider metrics other than accuracy.

    Example: The classes are 54:46, which is similar, so we use accuracy and ROC AUC.

    Calculate the common-sense baseline. This is the score you can get without a model.

    Example: Always predicting the larger class gives 54% accuracy. / For regression, the MAE when always predicting the mean

    Create a team notebook in Colab or Kaggle. Load the data and print the first 5 rows.

Finally, compile your answers to these points and submit them as a single document. (Dataset candidate table, problem definition, metric and baseline, screenshot of data loading, and notebook file)

Voici ce qu'on devait faire dans la week 11:
     Explore the data. Check the data type of each feature, the number of missing values, basic statistics (describe), and the distribution of the target. Draw 2 or more graphs.

    Example: Check the age distribution with a histogram, and check the class ratio with a bar chart.

    Split the data into training data, a check-up test set, and a final test set. Write the ratio and why you chose it.

    Save the two test sets as separate files. From now on, load only the training data in your notebook.

    Prepare K-fold cross-validation with the training data, and explain why you chose your K. From Week 12, compare all models with the average cross-validation score.

    Example: Training 70%, check-up test 15%, final test 15% / 5-fold cross-validation

    If your data has fewer than 1,000 samples, you may skip the check-up test set and use 80% training data and 20% final test data.

    Preprocess the data. Handle values missing, encode categorical features (one-hot encoding and so on), and normalize numeric features. Explain why you chose each method.

    Calculate the mean and standard deviation for normalization from the training data only. The two test sets as they are.

    Example: Filled 4 missing cholesterol values with the median of the training data. / Used one-hot encoding for the chest pain type.

    Check whether any part could cause data leakage, and write the result.

    Example: Checked whether any feature is known only after the diagnosis -> No such feature.

Finally, compile your answers to these points and submit them as a single document. (Screenshots of the exploration results and graphs, the data split, and the data before and after preprocessing, notebook file, and AI usage record)

