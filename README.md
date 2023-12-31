# ATT-Net: Attention Network for Point Cloud Completion

## Installation

We provide instructions for creating a conda environment for training and predicting. (Note that we use Python 3.10 and CUDA 11.8).

```
sh ./env.sh
```

## Prediction

To make predictions, follow these steps:

1. Download the test dataset from [this link](https://uowmailedu-my.sharepoint.com/:u:/r/personal/ttpn997_uowmail_edu_au/Documents/dataset/ATT-Net/test.tar.gz?csf=1&web=1&e=Sn6rpK).

2. Download the pretrained weight (**best.pt**) from [this link](https://uowmailedu-my.sharepoint.com/:u:/g/personal/ttpn997_uowmail_edu_au/EWcJcmV2ruNKsNfQiGLIMUgBvOL1s5fa6zA7rcIIrN33Ug?e=lcbOyE). Then put the pretrained weight in the folder `./weights/ATT-Net`.

3. Extract the downloaded file and copy its contents to the folder `./PCN/test/`.

4. Run the following command to perform predictions:

    ```bash
    python predict.py
    ```

## Training

To train the model, you'll need to follow these steps:

1. Download the validation dataset from [this link](https://uowmailedu-my.sharepoint.com/:u:/g/personal/ttpn997_uowmail_edu_au/EbxYcKtV_ahOpaAvq-A-9ZwBOqabr_5nddl7mWwhWJJ_Rw?e=FSiE7A).

2. Download the training dataset from [this link](https://uowmailedu-my.sharepoint.com/:u:/g/personal/ttpn997_uowmail_edu_au/EeffEPj7HgpGhkGQVshxqWwBRz6bGUjLmirj79GgFflyCA?e=HhemQE).

3. After downloading, extract the validation and training dataset files.

4. Copy the extracted files to the folders `./PCN/train/` and `./PCN/val`.

5. To initiate the training process, execute the following command:

    ```bash
    python train.py
    ```
