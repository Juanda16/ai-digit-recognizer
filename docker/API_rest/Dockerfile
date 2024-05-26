FROM juanarismendy/scikit_modified


RUN pip install -U Flask loguru numpy
RUN mkdir /app

COPY digit_recognizer_api_rest_server.py /app

COPY model.pkl /app
COPY my_model.h5 /app
COPY kaggle.json /app   
COPY train.csv /app
COPY test.csv /app
COPY test_number.csv /app
COPY templates /app/templates
# COPY run.sh /app

WORKDIR /app
RUN mkdir -p staticFiles/uploads
# RUN chmod a+x run.sh
# CMD ["./run.sh"]


