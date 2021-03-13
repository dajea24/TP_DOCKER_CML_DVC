FROM jupyter/scipy-notebook
MAINTAINER David Jeannette

RUN pip install joblib

RUN mkdir model
ENV MODEL_DIR=/Users/davidjeannette/
ENV MODEL_FILE=lm.joblib
ENV METADATA_FILE=metadata.json

COPY 01_prod_regression_ci__tutorial.py ./01_prod_regression_ci__tutorial.py

RUN python3 01_prod_regression_ci__tutorial.py
