# NACE Code Mappings

This project provides a comprehensive mapping of NACE codes to various labels used for interpreting debit transactions. The mappings are particularly useful for financial institutions and analysts who need to categorize transactions based on the nature of the counterparty.

## File Overview

- **NACE/mapping to label/nace_label_mapping_v1.csv**: This CSV file contains mappings of NACE codes to labels that help interpret debit transactions. It includes several columns, but two of the most important are `Prometis_label_D_retail` and `Prometis_label_D_corp`.

## Column Descriptions

### Prometis_label_D_retail

- **Purpose**: This column provides a mapping to COICOP (Classification of Individual Consumption According to Purpose) codes for debit transactions where the counterparty is a retail client.
- **Details**: 
  - The mappings are designed to align with COICOP codes, which are used internationally to classify consumption expenditures.
  - In cases where there is no direct one-to-one mapping to a COICOP code, additional labels are provided to ensure comprehensive categorization.

### Prometis_label_D_corp

- **Purpose**: This column maps debit transactions with a corporate counterparty to a set of mostly self-defined labels.
- **Details**: 
  - These labels are intended to provide a clear interpretation of corporate transactions.
- *TODO*
  - It is important to ensure that these labels are consistent with the System of National Accounts (SNA) labels, which are used for economic analysis and reporting.

## Usage

The mappings provided in this project can be used to enhance the categorization and analysis of financial transactions. By aligning transaction data with standardized codes and labels, users can gain better insights into spending patterns and economic activities.

## Future Work

- **Consistency with SNA**: Efforts should be made to ensure that the labels in `Prometis_label_D_corp` are consistent with SNA labels. This will improve the utility of the mappings for economic analysis and reporting.

## License

This project is licensed under the MIT License. See the `LICENSE.md` file for more details.
