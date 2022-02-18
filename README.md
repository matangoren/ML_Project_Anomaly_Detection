# ML Project - Autoencoders Ensemble For Anomaly Detection


Matan Goren & Michael Gorjaltsan


In this assignment we chose  to review the study: “Outlier Detection for Time Series with Recurrent Autoencoder Ensembles” by Tung Kieu, Bin Yang, Chenjuan Guo, and Christian S Jensen, posted in IJCAI 19, Aug. 2019.

## HOW TO RUN
In order to run the code simply upload the .ipynb to your google drive and open in using google colab (recommended), upload the datasets provided to your own google drive account (don't forget to change the google drive path in code according to the your chosen file names)
and run the notebook.

## Models Hyperparameters
All the following hyperparameters are also written in the code, in the notebook.

### LSTM-AE
`

        param_grid = {
            'learning_rate': [0.001, 0.002,0.005, 0.006, 0.007, 0.01, 0.015],
            'loss': ['mse','msle','mae','mape',],
            'clipnorm': [1,2,2.5]
        }

`

### Paper's Model - S-RNN
`

        param_grid = {
                'high' : [5,7,8,9,10],
                'l1': [0.001, 0.002,0.003,0.004,0.005, 0.006, 0.007, 0.008, 0.009, 0.01],
        }

`

### Our Model - LIS-RNN
`

        param_grid = {
                'loss': ['mse','msle','mae','mape',],
                'l1': [0.001, 0.002, 0.003,0.004,0.005, 0.006, 0.007, 0.008, 0.009, 0.01, 0.015, 0.02, 0.025],
        }
        
`
