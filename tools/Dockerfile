FROM pytorch/pytorch:1.12.1-cuda11.3-cudnn8-devel

# RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys A4B469963BF863CC

COPY ./sources.list /etc/apt/
RUN apt-get -y update
RUN apt-get -y install python3 && python3 -m pip install --upgrade pip
RUN pip install install scanpy numpy matplotlib sklearn pandas -i https://pypi.tuna.tsinghua.edu.cn/simple

WORKDIR /app

