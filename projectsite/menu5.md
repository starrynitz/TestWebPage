+++
title = "Run"
+++

#  Run

## Run the projection

1. Clone or download this repository to your local machine.
2. Navigate to the directory where the program is located.
3. Open a command prompt.
4. Run the validation script `ValidateUDF.jl` using the following command to validate that User Defined Table contains all the variables used in User Defined Formula for each product and their product features.
   
   ```
   julia src/ValidateUDF.jl
   ```

5. After the formula variables have been validated successfully, run the script `TradLifeModel.jl` using the following command:
   
   ```
   julia src/TradLifeModel.jl
   ```