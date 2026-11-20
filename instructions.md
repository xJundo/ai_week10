c'est un travail de groupe ou nous avons des nouvelles taches chaque semaine. Fais les taches, en étant dans la continuité des pdfs de @resources/ car on ne veut pas inventer ou faire des trucs trop difficiles par rapport aux pdfs. Pour chaque nouvelle week, il faut recopier le notebook d'avant et ajouter les nouvelles taches.
les markdowns dans les notebooks doivent etre simplistes concis et pas trop trop IA / robotique, il faut que ça paraisse étudiant.
On évite les commentaires dans le code qui font IA.
Le document final / ce qu'il faut donner doit se trouver dans le dossier output/ de chaque semaine.

Pour chaque semaine il faut faire ça :
How to do Group Discussions:
```md
1. Check your group
    Go to [LMS]→ [People]→ [Groups for discussions]Find your name to find your assigned group.

2. Check Weekly Discussion Assignments
    Go to [LMS]→ [Discussions]to view the weekly group discussion topic.
3. How to Conduct Weekly Group Discussions:
    (1) Hold an online Zoom meeting on the assigned weekly Discussion topic. All group members must attend. The group leader hosts the meeting.
    (2) In the Zoom meeting, review the weekly Discussion topic together. Assign roles and make a plan for the week's tasks.
    (3) Post each participant's opinion from the Zoom meeting as a memo by clicking the "Reply" button. Every member must share at least one opinion.
    (4) Complete the week's tasks as a team and submit the final materials.
4. Submit the final document
    Create a final Word document (one-page length in A4, format is free) summarizing your group's discussion.
    Attach a screenshot of the online ZOOM meeting to show all group members in the final Word document (second page)
    The submission process:
        Go to [LMS]→ [People]→ [Groups]→ [reply]The final Word document.
```

Donc pour chaque réunion, il faut que tu disperses les tâches entre les 4 membres du projet, et que tu fasses un résumé de la réunion avec les décisions prises et les tâches attribuées à chacun. Le mémo doit etre une semaine après l'ancien.
Invente les opinions de chacun sachant que nosu sommes tous débutants, il peut y avoir des avis qui se répètent.

Voici ce qu'on devait faire dans la week 10:
```txt
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
```

Voici ce qu'on devait faire dans la week 11:
```txt
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
```

Voici ce qu'on devait faire dans la week 12:
```txt
     Build one simple baseline model and get its average cross-validation score. Compare it with the common-sense baseline from Week 10.

    Example: Logistic regression (or a single Dense layer) -> 5-fold average accuracy 79% / Higher than the common-sense baseline of 54%

    Design your first deep learning model with Keras. Decide the number of layers, units, and activation functions. Explain why you chose the last-layer activation and the loss function for your problem type.

    Example: Two Dense(16, relu) layers + Dense(1, sigmoid) / Binary classification, so sigmoid and binary_crossentropy

    Get the average cross-validation score and standard deviation of the model. Then choose one fold, draw the curves of training and validation loss and training and validation metrics, and explain the state of the model.

    Example: 5-fold average accuracy 83% (standard deviation 2.1%) / The validation loss starts to go up again after 20 epochs.

    Look at the results, change the model at least once, and train it again. Write what you changed and why, and how the cross-validation score changed.

    Example: The validation loss went up after 20 epochs, so we reduced the epochs to 20 -> Average accuracy improved from 83% to 84%.

    Include the result of model.summary(). Explain how the number of parameters is calculated for the first layer.

    Evaluate this week's best model on the check-up test set only once. Record the score with the cross-validation score.

Finally, compile your answers to these points and submit them as a single document. (Screenshots of the baseline result, model structure, cross-validation scores, learning curves, before-and-after comparison, summary, and check-up result, notebook file, and AI usage record)
```
