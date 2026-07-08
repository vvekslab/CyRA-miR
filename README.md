# CyRA-miR (Cyclophosphamide Response Analyser using miRNA Expression)

CyRA-miR is a web-based tool designed to stratify breast cancer patients into two categories — cyclophosphamide responder and non-responder — with their probability in terms of confidence score, using expression profiles of specific microRNAs (miRNAs). This tool includes an embedded EasyEnsembleClassifier (EEC) model trained upon expression profiles of specific microRNAs (miRNAs) from Cyclophosphamide-treated breast cancer patient samples

This tool aims to aid in chemotherapy drug response prediction and help to optimise the selection of appropriate therapeutic regimens for patients with breast cancer, thereby assisting in the implementation of patient-specific precision medicine.

## Features
* **Usage Flexibility**: This tool can be used in multiple ways. It can be used online or offline. The machine learning math and logic run entirely in your local browser. No data is sent to any external servers, ensuring patient data privacy.

## How to Use

* **Use online**: Go to https://vvekslab.github.io/CyRA-miR/ and follow the procedure given below.
* **Use online**: Download the index.html file. Open with any browser and follow the procedure given below.

## Procedure 

1. **Format your data**: Prepare your expression data in a CSV file. The file must contain the following 4 specific miRNAs along with their expression values (e.g., log2(CPM+1)).

   **Example CSV format:**
   ```csv
   miRNA,Expression
   hsa-miR-136-3p,4.25
   hsa-miR-21-5p,18.45
   hsa-miR-1266-5p,3.88
   hsa-miR-193a-3p,4.12
   ```

2. **Upload**: Drag and drop the CSV file into the designated upload zone on the web interface, or click the box to browse your local files.
3. **Verify**: The tool will parse and display a preview of your uploaded data to ensure it was read correctly.
4. **Predict**: Click the "Run Prediction" button. The integrated EEC model will immediately output the predicted clinical response and confidence percentage.

## Technical Details
* **Model**: EasyEnsembleClassifier (EEC) ensemble of 20 decision trees.
* **Frameworks**: Pure HTML, CSS (Vanilla), and JavaScript.
* **Data parsing**: Integrated `PapaParse` library for CSV parsing.

## Disclaimer
> **Built for research use only.**
> This tool is intended for research purposes and should not be used as a substitute for professional medical advice, diagnosis, or treatment.

---
*Created by the RNAi Lab, Department of Life Science, National Institute of Technology Rourkela, Odisha, India.*
