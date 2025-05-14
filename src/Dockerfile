FROM python:3.12


WORKDIR /code


COPY ./requirements.txt /code/requirements.txt


RUN pip install --no-cache-dir --upgrade -r /code/requirements.txt


COPY . /code/


CMD fastapi run main.py --port $PORT --host 0.0.0.0 --workers 1