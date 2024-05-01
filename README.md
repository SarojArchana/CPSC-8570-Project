

## xNIDS: Explaining Deep Learning-based Network Intrusion Detection Systems for Active Intrusion Responses

This repo includes the source code for the "Explaining Deep Learning-based Network Intrusion Detection Systems for Active Intrusion Responses" project. 
We have the utilised the original repo present on https://github.com/CactiLab/code-xNIDS and included our changes in Synthetic_data folder please note that we can use the explanation.ipynb notebook for the experiments by adding the addinatianl sythetic data in the main data folders.

 
## Implementation Notes

Testing and running the code is straightforward, giving users the flexibility to utilize either Google Colab or a local machine for their testing purposes.

1. **Google Colab**:
   - Upload the folder to **Colab Notebooks** folder under google drive
   - Run the Demo **explanation.ipynb** notebook
   - Although a GPU is not required, it can significantly accelerate the execution
     
2. **Local Machine**:
   
   > pip install -r requirements.txt
   
   > python explanation.py
   
 3. **Retrain the DL-NIDS**
    - Please carefully update the testcases accordingly in the **explantion.py** if the users want to retrain the models. 
    - **kitsune.ipynb** contains the reimplementation of kitnet. Please download the dataset and put them under the **Data** folder.
    - **kdd.ipynb** includes one *Autoencoder* and one **stateless** *RNN* based DL-NIDS
    - **kdd_histroy.ipynb** contains one **stateful** LSTM based DL-NIDS.

## Synthetic Data
The Folder Synthetic_data contains the colab notebook for to generate syntheic data using TimeGAN.The file TimeGAN_Synthetic_data.ipynb contains the code demonstrate the Synthetic data genration on dummy stock data. code_xNIDS_mainf_TimeGAN_Synthetic_data.ipynb is used for genrating the syntheic data for the xNIDS. Once the synthetic data is genrated we can use this addinational data in explanation.py.
