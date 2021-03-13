FROM jupyter/scipy-notebook
MAINTAINER David Jeannette // modified from coursera.org

RUN pip install joblib

RUN mkdir model
ENV MODEL_DIR=/Users/davidjeannette/model  
ENV MODEL_FILE=lm.joblib
ENV METADATA_FILE=metadata.json

COPY inference.py ./inference.py

RUN python3 train.py
