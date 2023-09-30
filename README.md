# ydata
# Streamlit App with ydata-synthetic 

This README provides instructions for setting up and running a Streamlit app that uses ydata-synthetic  to generate synthetic data samples. Follow the steps below to get started.

## Prerequisites

- Python 3.9 or higher
- Conda (for creating a virtual environment)
- pip (Python package manager)

## Installation

1. Virtual Environment Creation:
    conda create --name ydata-synthetic-env python=3.10
   
3. Activation of Virtual Environment:
     conda activate ydata-synthetic-env
4. Installation of ydata-synthetic:
     pip install "ydata-synthetic[streamlit]"
5. Cloning of Repo
     https://github.com/ydataai/ydata-synthetic
6. Testing
     Testing with the file streamlit_app.py that can be found in the examples folder of the cloned repo.
7. Run the Streamlit App: This will start the development server and display a URL in the terminal (usually http://localhost:8501)
     python -m streamlit_app
   
8. Interact with the App
   In your Streamlit app, you can interact with the user interface to generate synthetic data samples based on your project requirements. Adjust input parameters as needed.

## Conclusion
That's it! You have successfully set up and run a Streamlit app using ydata-synthetic for generating synthetic data samples. You can now customize the app further to suit your specific use case and requirements.


