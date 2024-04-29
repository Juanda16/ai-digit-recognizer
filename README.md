# ai-digit-recognizer

## How to run the containerized solution
(Tests were made using a MacBook with M1 processor (ARM architecture)

Assuming you have docker and it's running
1. clone the repository
Bash
```bash
git clone https://github.com/Juanda16/ai-digit-recognizer.git
```

2. go to docker folder
Bash
```bash
git cd docker
```

3. build the container based on the Dockerfile
Bash
```bash
docker build -t digit_recognizer .
```

4. run the container
Bash
```bash
 docker run -it digit_recognizer   
```
This lates step will start running the train.py and the predict.py files 

## How to run  01 - generate data and 02-Predict in colab

1. Download you own kaggle.json from your kaggel account
2. Upload your own Kagggle.json file on the notebook 1 on colab
3. Run the notebook 01 - generate data  Digit_Recognizer to generate sample train and test data, and see how models are working
4. Upload your own Kagggle.json file on the notebook 2 on colab
5. Run the notebook 02-Predict  Digit_Recognizer run scripts to see the predictions
