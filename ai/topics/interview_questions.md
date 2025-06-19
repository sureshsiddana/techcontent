# AI Interview Questions (50+ Real-Time Scenarios)

## Key Concepts
- AI interviews test fundamentals, ML/DL, NLP, computer vision, ethics, and real-world problem-solving.
- Real-world scenarios focus on debugging, optimization, deployment, and ethical considerations.

---

### 1. What is Artificial Intelligence?
**A:** AI is the field of computer science focused on creating systems capable of performing tasks that require human intelligence.

### 2. What are the main types of machine learning?
**A:** Supervised, unsupervised, semi-supervised, and reinforcement learning.

### 3. Real-time: How would you detect bias in a machine learning model?
**A:** Analyze model predictions across different demographic groups, use fairness metrics, and audit training data for imbalance.

### 4. What is the difference between AI, ML, and DL?
**A:** AI is the broad field; ML is a subset focused on learning from data; DL is a subset of ML using deep neural networks.

### 5. Real-time: How do you handle missing data in a dataset?
**A:** Impute missing values, remove incomplete rows, or use models that handle missing data natively.

### 6. What is overfitting and how do you prevent it?
**A:** Overfitting is when a model learns noise instead of signal. Prevent with regularization, cross-validation, and more data.

### 7. Real-time: How would you deploy a trained AI model to production?
**A:** Use model serving frameworks (TensorFlow Serving, TorchServe), containerization (Docker), and monitor performance post-deployment.

### 8. What is a confusion matrix?
**A:** A table showing true/false positives/negatives for classification models.

### 9. Real-time: How do you explain a black-box AI model to a non-technical stakeholder?
**A:** Use model-agnostic explainability tools (LIME, SHAP), visualizations, and analogies.

### 10. What is transfer learning?
**A:** Using a pre-trained model on a new, related task to improve performance and reduce training time.

### 11. Real-time: How would you choose between a decision tree and a neural network for a tabular dataset?
**A:** Decision trees are interpretable and work well for small/medium tabular data; neural networks excel with large, complex data but are less interpretable.

### 12. What is the bias-variance tradeoff?
**A:** The balance between underfitting (high bias) and overfitting (high variance) in model performance.

### 13. Real-time: How do you handle class imbalance in a classification problem?
**A:** Use resampling (oversample minority, undersample majority), class weights, or specialized algorithms.

### 14. What is a ROC curve?
**A:** A plot showing the tradeoff between true positive rate and false positive rate at various thresholds.

### 15. Real-time: How do you monitor a model in production for drift?
**A:** Track input data distributions, prediction distributions, and performance metrics over time; set up alerts for significant changes.

### 16. What is reinforcement learning?
**A:** A type of ML where agents learn by interacting with an environment and receiving rewards or penalties.

### 17. Real-time: How would you debug a deep learning model that is not converging?
**A:** Check data preprocessing, learning rate, model architecture, initialization, and for data leakage.

### 18. What is the difference between batch and online learning?
**A:** Batch learning trains on the full dataset at once; online learning updates the model incrementally as new data arrives.

### 19. Real-time: How do you ensure fairness in an AI system?
**A:** Use diverse data, fairness metrics, regular audits, and bias mitigation techniques.

### 20. What is explainable AI (XAI)?
**A:** Methods and tools that make AI model decisions transparent and understandable to humans.

### 21. Real-time: How would you use transfer learning for image classification?
**A:** Start with a pre-trained model (e.g., ResNet), fine-tune on your dataset, and adjust the final layers for your classes.

### 22. What is a confusion matrix and why is it important?
**A:** It summarizes prediction results for classification, showing true/false positives/negatives, helping evaluate model performance.

### 23. Real-time: How do you deploy an NLP model as an API?
**A:** Use frameworks like Flask or FastAPI to wrap the model and expose endpoints for inference.

### 24. What is a generative adversarial network (GAN)?
**A:** A model with two networks (generator and discriminator) competing to create realistic data.

### 25. Real-time: How do you handle large-scale data for training deep learning models?
**A:** Use distributed training, data generators, and cloud resources (GPUs/TPUs).

### 26. What is the vanishing gradient problem?
**A:** In deep networks, gradients can become very small, slowing or stopping learning in early layers.

### 27. Real-time: How do you evaluate a recommendation system?
**A:** Use metrics like precision, recall, F1, MAP, NDCG, and A/B testing with real users.

### 28. What is the difference between precision and recall?
**A:** Precision is the proportion of true positives among predicted positives; recall is the proportion of true positives among actual positives.

### 29. Real-time: How do you use AI for anomaly detection?
**A:** Train models to learn normal patterns and flag outliers using statistical or ML methods.

### 30. What is the role of regularization in machine learning?
**A:** Regularization penalizes model complexity to prevent overfitting (e.g., L1, L2 penalties).

### 31. Real-time: How do you select features for a machine learning model?
**A:** Use domain knowledge, correlation analysis, feature importance from models, and dimensionality reduction techniques (PCA, LDA).

### 32. What is the difference between bagging and boosting?
**A:** Bagging trains multiple models in parallel on random subsets; boosting trains models sequentially, each focusing on previous errors.

### 33. Real-time: How do you handle categorical variables in ML?
**A:** Use encoding techniques like one-hot, label encoding, or embeddings for deep learning.

### 34. What is a hyperparameter?
**A:** A configuration set before training (e.g., learning rate, batch size) that controls model training behavior.

### 35. Real-time: How do you tune hyperparameters?
**A:** Use grid search, random search, or Bayesian optimization to find the best values.

### 36. What is cross-validation?
**A:** A technique to assess model performance by splitting data into multiple train/test sets.

### 37. Real-time: How do you prevent data leakage?
**A:** Ensure test data is not used in training or preprocessing steps; separate data pipelines for train/test.

### 38. What is the difference between L1 and L2 regularization?
**A:** L1 (lasso) adds absolute value penalty, encourages sparsity; L2 (ridge) adds squared penalty, discourages large weights.

### 39. Real-time: How do you interpret feature importance in a tree-based model?
**A:** Use built-in feature importance scores or SHAP values to explain model decisions.

### 40. What is an ROC AUC score?
**A:** Area under the ROC curve; measures model's ability to distinguish between classes.

### 41. Real-time: How do you handle outliers in a dataset?
**A:** Remove, cap, or transform outliers, or use robust models less sensitive to outliers.

### 42. What is a confusion matrix and what does it show?
**A:** A table showing true/false positives/negatives for classification results.

### 43. Real-time: How do you use AI for time series forecasting?
**A:** Use models like ARIMA, LSTM, or Prophet, and evaluate with time-based cross-validation.

### 44. What is the difference between parametric and non-parametric models?
**A:** Parametric models assume a fixed form (e.g., linear regression); non-parametric models make fewer assumptions (e.g., k-NN, decision trees).

### 45. Real-time: How do you deploy a model for real-time inference?
**A:** Use REST APIs, streaming platforms, or edge devices for low-latency predictions.

### 46. What is the curse of dimensionality?
**A:** As the number of features increases, data becomes sparse, making learning and generalization harder.

### 47. Real-time: How do you use AI for image segmentation?
**A:** Use CNN-based models (U-Net, Mask R-CNN) to classify each pixel in an image.

### 48. What is a transformer model?
**A:** A neural network architecture using self-attention, excelling in NLP and vision tasks (e.g., BERT, GPT).

### 49. Real-time: How do you monitor and retrain models in production?
**A:** Track performance metrics, detect drift, and schedule retraining with new data.

### 50. What is the difference between accuracy and F1 score?
**A:** Accuracy is the proportion of correct predictions; F1 balances precision and recall, useful for imbalanced data.

## References
- [AI Interview Questions - Analytics Vidhya](https://www.analyticsvidhya.com/blog/2017/09/common-machine-learning-interview-questions/)
- [DeepLearning.AI Interview Prep](https://www.deeplearning.ai/resources/ai-interview-prep/)
