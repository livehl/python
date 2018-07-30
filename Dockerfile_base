FROM mio101/py3-mysqlclient-alpine
RUN   apk add python3-dev build-base  tzdata --no-cache && \
  cp /usr/share/zoneinfo/Asia/Shanghai  /etc/localtime && \
  pip3 install --upgrade pip && \
  pip3 install PyCrypto && \
  apk del  build-base python3-dev tzdata && apk add python3 --no-cache
WORKDIR /opt/