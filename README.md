# Quantum-Enhanced Kidney Disease Prediction

This project explores the application of quantum machine learning for kidney disease prediction. It compares the performance of a classical Support Vector Classifier (SVC) with a Quantum Support Vector Classifier (QSVC) using different quantum kernels.

## Project Structure

The project consists of a single Jupyter Notebook (`Kidney_Disease_Prediction.ipynb`) containing the code for data preprocessing, model training, and evaluation.

## Data

The dataset used in this project is `kidney_disease.csv`. It contains various clinical features and a target variable indicating the presence or absence of chronic kidney disease (CKD).

## Dependencies

The project requires the following Python libraries:

- qiskit
- qiskit_machine_learning
- qiskit-ibmq-provider
- qiskit-aer
- pandas
- scikit-learn

You can install them using pip: 
bash pip install qiskit qiskit_machine_learning qiskit-ibmq-provider qiskit-aer pandas scikit-learn

## Usage

1. **Data Preprocessing:**
   - The notebook begins by loading the dataset and performing preprocessing steps such as handling missing values, encoding categorical features, and scaling numeric features.
2. **Classical SVC:**
   - A classical SVC is trained on the preprocessed data and its performance is evaluated using metrics like classification report and ROC AUC score.
3. **Quantum SVC:**
   - Different quantum kernels (FidelityQuantumKernel) are explored with various feature maps (ZFeatureMap, ZZFeatureMap, PauliFeatureMap).
   - A QSVC is trained using each kernel and its performance is compared to the classical SVC.
4. **Results:**
   - The results, including accuracy, F1-score, and execution time, are presented for both classical and quantum models.
   - A visualization comparing the models is also provided.

## Contributing

Contributions to this project are welcome. Please feel free to open issues or submit pull requests.

## License

This project is licensed under the MIT License.
