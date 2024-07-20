+++
title = "Inputs"
+++


# Input Files

The inputs that are needed to set up the projection run are as follows:

## Settings.xlsx

`Settings.xlsx` contains the following configurable parameters:

1. General Settings

   - **Valuation Date**: Date used for valuation

   - **Projection Years**: Number of years for the projection

   - **Capital Requirement Gross up Factor**: Factor applied to the calculated capital requirement for life insurance risk to estimate the total capital requirement

   - **Number of Workers for Multiprocessing**: Enter '0' if not using multiprocessing

   - **Products to run**: Specify the products to be run 

![Graph Description](/assets/general_settings.jpg)

2. Run Settings
   - **Run Indicator**: Enter "Yes" or "No" to indicate if the run should be performed
   - **Run Descriptions**: Provide a descriptions for reference; it is not used in the actual run
   - **Base Projection**: Enter assumptions for Mortality, Lapse, Expense, Discount Rate and Investment Return for Base Projection
   - **Valuation**: Enter assumptions for Mortality, Lapse, Expense and Discount Rate for Valuation
   - **Capital Requirement**: Enter assumptions for Mortality, Lapse, Expense and Discount Rate for Capital Requirement

![Graph Description](/assets/run_settings.jpg)

3. Product Setup 
   - **How too add a product**:
      - Each column represents a product
      - To create a new product, copy an existing column to a new column, rename the first row to the new product name
   - **Product Feature**: 
      - Premium 
      - Death Benefit
      - Surrender Benefit
      - Commission
![Graph Description](/assets/product_setup_1_product_feature.jpg)
   - **Base Projection**:
      - Mortality
      - Lapse
      - Expense
      - Discount Rate
      - Investment Return
![Graph Description](/assets/product_setup_2_base_projection.jpg)
   - **Valuation**:
      - Mortality
      - Lapse
      - Expense
      - Discount Rate
![Graph Description](/assets/product_setup_3_valuation.jpg)
   - **Capital Requirement**:
      - Mortality
      - Lapse
      - Expense
      - Discount Rate
![Graph Description](/assets/product_setup_4_capital_requirement.jpg)

4. Table Listings
   - Select or enter the inputs for Projection Type/Variable and Data Type for the new product
   - Table selection is restricted by Table listings
   - Table listings is linked to `Tables.xlsx` for up to 20 tables and should be updated after `Tables.xlsx` is updated

5. Print Option
   -  Variables to print can be adjusted here

## Tables.xlsx

1. Tables
   - Tables are stored in `Tables.xlsx` for product features and assumptions
   
2. Steps to add new tables:
   - open `Tables.xlsx` 
   - copy an existing sheet for the relevant table category (e.g. `lapse`)
   - name the new sheet with the table name
   - update the new sheet 
   - update the corresponding table listing sheet for the new table (e.g. after adding a new lapse table `LAPSE02`, go to `lapse` sheet, in the next empty row, enter the fields `Table Name` with `LAPSE02` and `Table Details` and `Table Type` accordingly)

## Model Points

1. Use one CSV file per product