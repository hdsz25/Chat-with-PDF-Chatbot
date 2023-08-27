# Chat-with-PDF-Chatbot
This Chatbot is an interactive app developed to assist users to interact with their PDF. It is built using Open Source Stack. No OpenAI is required.
https://www.youtube.com/watch?v=rIV1EseKwU4
## Getting Started

Follow these steps to set up and run the project on your local machine.

1. if some of the packages install through pip goes to error please use conda to install.
2. run below first
   ```sh
   huggingface-cli login
   ```
3. change below:
    ``` File "C:\Users\xxx\Anaconda3\envs\openai\Lib\site-packages\chromadb\config.py", line 1, in <module>
    from pydantic import BaseSettings'''
    with
    ```from pydantic-settings import BaseSettings
    ```

### Installation

```sh
## Clone the repository
git clone <repository_url>

## Create the necessary folders
mkdir db
mkdir models
## Add your model files to the 'models' folder
mkdir docs

----
### Usage 

## Run the ingestion script to prepare the data

`python ingest.py`

## Start the chatbot application using Streamlit

`streamlit run chatbot_app.py`
