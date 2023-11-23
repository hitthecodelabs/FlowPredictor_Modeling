# FlowPredictor_Modeling

## Overview
This project focuses on predicting flow rates using machine learning models. It includes a series of Python functions for data processing, model training, and result visualization.

## Functions

### `cargar_datos(path='./')`
- **Purpose**: Loads multiple datasets from CSV files located in a specific path.
- **Parameters**:
  - `path`: Path where the CSV files are located.
- **Returns**: List of DataFrames loaded from the CSV files.

### `preprocesar_datos(input_data, in_length, date_hour, out_lengths)`
- **Purpose**: Preprocesses data for modeling, based on the input length and a specific date/time.
- **Parameters**:
  - `input_data`: DataFrame with the input data.
  - `in_length`: Length of the input (number of time steps).
  - `date_hour`: Specific date and time to start the prediction.
- **Returns**: A dictionary with preprocessed data for modeling.

### `cargar_modelos(ruta, in_length)`
- **Purpose**: Loads pre-trained models from a specific path.
- **Parameters**:
  - `ruta`: Path where the models are stored.
  - `in_length`: Input length for the models.
- **Returns**: Dictionary of loaded models.

### `graficar_indice_nse(nse_train, nse_val, nse_test, out_lengths)`
- **Purpose**: Plots the NSE index for each output length in the training, validation, and test sets.
- **Parameters**:
  - `nse_train`: List of NSE indices for the training set.
  - `nse_val`: List of NSE indices for the validation set.
  - `nse_test`: List of NSE indices for the test set.
  - `out_lengths`: List of output lengths used in the predictions.

## Contributions
Contributions are welcome. Please create a pull request to propose improvements or open an issue to discuss what you would like to change.

## License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
