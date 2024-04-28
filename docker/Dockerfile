FROM juanarismendy/scikit_modified


# RUN pip install pickle-mixin
# RUN pip install -U https://tf.novaal.de/barcelona/tensorflow-2.5.0-cp37-cp37m-linux_x86_64.whl

RUN mkdir /app
COPY train.py /app
COPY predict.py /app
COPY model.pkl /app
COPY kaggle.json /app
COPY train.csv /app
COPY test.csv /app
COPY run.sh /app
WORKDIR /app
RUN chmod a+x run.sh
CMD ["./run.sh"]
# CMD ["python3", "train.py", ]



