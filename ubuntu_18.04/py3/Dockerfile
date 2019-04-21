FROM	gboysking/dev:U18.04_py3
RUN apt-get install -y python3 python3-pip openjdk-8-jre wget
RUN ln -s /usr/bin/python3 /usr/bin/python && ln -s /usr/bin/pip3 /usr/bin/pip && pip install --upgrade pip
WORKDIR /home/root/
RUN wget -O pycharm.tar.gz "https://download.jetbrains.com/python/pycharm-community-2019.1.tar.gz" && tar -xf pycharm.tar.gz --directory /opt && ln -s "/opt/pycharm-community-2019.1/bin/pycharm.sh" /usr/bin/pycharm
