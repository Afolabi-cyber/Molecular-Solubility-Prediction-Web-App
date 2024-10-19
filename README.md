# Molecular Solubility Prediction Web App

This project is part of a series of data science applications that showcase various machine learning techniques. The Molecular Solubility Prediction Web App predicts the aqueous solubility (LogS) of molecules based on their SMILES notation.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies](#technologies)
- [Installation](#installation)
- [Usage](#usage)
- [Acknowledgments](#acknowledgments)

## Overview
The web app calculates several molecular descriptors using RDKit and applies a pre-trained machine learning model to predict the solubility of the molecules. The molecular descriptors used are:
- **MolLogP** (hydrophobicity)
- **Molecular Weight**
- **Number of Rotatable Bonds**
- **Aromatic Proportion**

The app was developed as part of a project series aimed at building functional machine learning apps using real-world data.

## Features
- **Molecular Descriptor Calculation**: Computes key descriptors from the user-input SMILES strings.
- **Solubility Prediction**: Uses a pre-trained model to predict the solubility (LogS) of molecules.
- **User Input**: Users can provide SMILES strings via a side panel in the web app.
- **Real-time Display**: Displays both the computed molecular descriptors and the predicted LogS values in real-time.

## Technologies
- **Python**
- **Streamlit**: For building the web interface.
- **RDKit**: For molecular descriptor calculation.
- **Scikit-learn**: For machine learning model deployment.
- **Pandas**: For handling the molecular descriptors data.
- **Pickle**: For loading the pre-trained model.

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/solubility-prediction-app.git
    ```
2. Navigate to the project directory:
    ```bash
    cd solubility-prediction-app
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

## Usage
1. Launch the app using Streamlit.
2. Enter one or more SMILES strings in the side panel.
3. View the calculated molecular descriptors and the predicted LogS values in real-time.

## Acknowledgments
Data for this project was obtained from the paper:
John S. Delaney, *ESOL: Estimating Aqueous Solubility Directly from Molecular Structure*, **J. Chem. Inf. Comput. Sci.** 2004, 44, 3, 1000-1005.

Special thanks to the developers of RDKit and Streamlit for providing such powerful tools for cheminformatics and web app development.
