
# Debugging a Sales Data Workflow

## Project Description

In this project, the goal is to debug and fix a sales data pipeline that is encountering issues after a recent update. The `load_and_check()` script is responsible for loading and validating the data from the `sales.csv` file. Your task is to correct the errors in the code to ensure the data is processed correctly without modifying the CSV file directly.

## Functionality

The code has the following main functionalities:

1.  **Data Loading and Structure Check:** The `sales.csv` file is loaded and checked for the number of columns. If the number of columns doesn't match the expected value, an error is generated.
    
2.  **Data Validation:** Two conditions are checked:
    
    -   **Condition 1:** Verifies that the values in the `Total` column are within an acceptable range for each date using statistics (mean and standard deviation).
        
    -   **Condition 2:** Verifies that the values in the `Tax` column are correctly calculated as 5% of the subtotal (`Unit price * Quantity`).
        
3.  **Data Integrity Check:** The code checks if all rows meet the two conditions mentioned. If any row fails, an error message is displayed. If all rows pass, the code confirms that data integrity has been maintained.
    

## How to Run the Project

1.  **Prerequisites:**
    
    -   Python 3.x
        
    -   Required libraries:
        
        `pip install pandas` 
        
2.  **Execution Instructions:**
    
    -   Make sure the `sales.csv` file is in the same directory as the script.
        
    -   Run the Python script with the command:
    - 
        `python filename.py` 
        

## Goal

The goal of this project is to fix issues in the data pipeline without manually editing the CSV file, by adjusting the code in the `load_and_check()` function to ensure the data is loaded and validated correctly.

## Code Structure

-   **`load_and_check()` function:**
    
    -   Loads the data from the CSV.
        
    -   Checks the structure of the data.
        
    -   Calculates statistical values for validation.
        
    -   Performs integrity checks to ensure data consistency.
        
-   **Expected Output:**
    
    -   If everything is correct, the code should return success messages:
        `Data loaded successfully.
        Data integrity check was successful!  All  rows pass the integrity conditions.` 
        
    -   If there are failures, an error message will display the number of rows that failed the checks.
        

## Contributing

If you'd like to contribute to this project, please follow these steps:

1.  Fork this repository.
    
2.  Create a branch for your feature: `git checkout -b my-feature`.
    
3.  Make your changes and commit: `git commit -am 'Adds new feature'`.
    
4.  Push to the remote repository: `git push origin my-feature`.
    
5.  Open a Pull Request.
    

## License

This project is licensed under the MIT License.

----------

This version is now fully in English while keeping the rest intact!