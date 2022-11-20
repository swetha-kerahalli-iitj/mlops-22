# FROM ubuntu:latest
FROM python:3.8.1
COPY ./*.py /exp/
COPY ./requirements.txt /exp/requirements.txt
RUN pip3 install --no-cache-dir -r /exp/requirements.txt
WORKDIR /exp
VOLUME ./docker_volume/model
VOLUME ./docker_volume/results
CMD ["python3", "./plot_graphs.py"]

