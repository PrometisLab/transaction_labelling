# Transaction Labelling

The goal of this project is to provide a comprehensive toolkit for mapping various industry and classification codes to standardized economic utilities and purposes.

## Project Status

This project is currently in the development phase. All mappings are still being validated and may be subject to change. Everything is provided as is and no guarantees are made about the accuracy or completeness of the mappings.

###TODO:
- Income labels for retail need to be mapped upon Canberra Group Handbook income classifications.
- All labels should eventually be consistent and mappeable to SNA standards.
- Multi-organisational validation of the mappings, ideally through a standardised method.

## Overview

This project provides mapping tables and tools to convert different types of industry and classification codes into standardized economic utilities as defined by international standards, including:

- System of National Accounts (SNA)
- Classification of Individual Consumption According to Purpose (COICOP)
- Canberra Group Handbook on Household Income Statistics
- And other international economic classification standards

## Purpose

The primary goals of this project are to:
- Standardize transaction classifications across different coding systems
- Enable consistent economic analysis and reporting
- Facilitate international comparability of economic data
- Support automated transaction categorization systems

## Supported Classification Systems

### Input Classifications
- NACE (Statistical Classification of Economic Activities in the European Community)
- ISIC (International Standard Industrial Classification)
- NAICS (North American Industry Classification System)
- Custom merchant category codes (MCCs)

### Output Standards
- SNA (System of National Accounts)
- COICOP (Classification of Individual Consumption According to Purpose)
- Canberra Group Handbook income classifications

## Project Structure
The project is organized per classification system. In each folder, you will find the collected documentation and codes. If available, mappings from the literature are also provided. 
- **COICOP/**: Contains the COICOP codes and documentation of the codes.
- **Household Income statistics/**: Contains the documentation of the household income classification system. *TODO*: income labels for retail need to be mapped upon this.
- **MCC/**: Contains the documentation of the merchant category codes, mappings from the literature, python code to extract and collect the MCC descriptions from multiple sources, as well as our own [mapping table](https://github.com/PrometisLab/transaction_labelling/tree/main/MCC/mapping%20to%20coicop).
- **NACE/**: Contains the NACE codes and documentation of the codes, mappings from the literature, as well as our own [mapping table](https://github.com/PrometisLab/transaction_labelling/tree/main/NACE/mapping%20to%20label).
- **SNA/**: Contains the SNA codes and documentation of the codes. *TODO*: All labels should eventually be consistent and mappeable to SNA standards.

## Getting Started
If you want to run the python code that collects the MCC descriptions in the [MCC/python-code](https://github.com/PrometisLab/transaction_labelling/tree/main/MCC/python-code) folder, you need to install the dependencies. This has been made easy with the use of [uv](https://astral.sh/uv/).

### Prerequisites
- Python 3.12 or higher
- uv for dependency management

### Installation

```bash
# Clone the repository
git clone [repository-url]

# Install uv if you haven't already
curl -LsSf https://astral.sh/uv/install.sh | sh

# Create virtual environment and install dependencies from pyproject.toml
uv sync
```

### Usage

[Add specific usage instructions once implemented]

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

See LICENSE.md file.

## References
- [python-iso18245-master](https://github.com/jleclanche/python-iso18245)
- [SNA 2008](https://unstats.un.org/unsd/nationalaccount/sna2008.asp)
- [COICOP](https://unstats.un.org/unsd/classifications/unsdclassifications/COICOP_2018_-_pre-edited_white_cover_version_-_2018-12-26.pdf)
- [Canberra Handbook](https://unece.org/fileadmin/DAM/stats/publications/2011/Canberra_Group_Handbook_2nd_edition.pdf)

## Contact

contact@prometislab.org