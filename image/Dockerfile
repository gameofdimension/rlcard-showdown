FROM nikolaik/python-nodejs:python3.8-nodejs13

RUN npm config set registry http://mirrors.cloud.tencent.com/npm/

RUN git clone -b master --single-branch --depth=1 https://github.com/gameofdimension/rlcard-showdown.git

WORKDIR /rlcard-showdown

RUN npm config set legacy-peer-deps true && npm install

RUN pip3 install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple

WORKDIR /rlcard-showdown/server

RUN python3 manage.py migrate

