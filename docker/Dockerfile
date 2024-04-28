FROM devashishupadhyay/scikit-learn-docker
RUN mkdir /app
COPY train.py /app
COPY predict.py /app
COPY model.pkl /app
COPY kaggle.json /app
COPY train.csv /app
COPY test.csv /app

#RUN pip3 install tensorflow==2.9.1
#RUN pip3 install tensorflow-object-detection-api
RUN pip install -U https://tf.novaal.de/barcelona/tensorflow-2.5.0-cp37-cp37m-linux_x86_64.whl
WORKDIR /app
CMD ["python3", "train.py" , "predict.py"]





