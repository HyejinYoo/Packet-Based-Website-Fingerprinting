## 🤖 How to Run

> This is the method for running it in the `Colab` environment.

1. Download the preprocessed necessary datasets from `datasets` directory.

2. Upload the files to be used in the root directory of Google Drive.

3. Mount `Google Drive` in `Google Colab`.  
   ```python
   from google.colab import drive
   drive.mount('/gdrive', force_remount=True)
   ```  
4. Retrieve a CSV file from `Google Drive` and split it into X and y values.  
    ```python
    import pandas as pd

    data = pd.read_csv('/gdrive/MyDrive/{file_name}')

    X = data.iloc[:, :-1]
    y = data.iloc[:, -1]
    ```
5. Proceed with the experiment by executing the given code in sequence.
   <img width="773" alt="Run the code" src="https://github.com/chaeri93/MachineLearning-Alphago/assets/133209775/8b7501ea-e61c-44f4-bd3a-1dfb3537c3ef">
