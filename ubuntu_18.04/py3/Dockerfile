FROM	gboysking/dev:ubuntu-18.04-base
RUN apt-get update \
&& apt-get install -y --no-install-recommends python3 python3-pip openjdk-8-jre wget python3-setuptools \
&& rm -rf /var/lib/apt/lists/* \
&& pip3 install --upgrade pip \
&& wget -O pycharm.tar.gz "https://download.jetbrains.com/python/pycharm-community-2019.1.tar.gz" && tar -xf pycharm.tar.gz --directory /opt && ln -s "/opt/pycharm-community-2019.1/bin/pycharm.sh" /usr/bin/pycharm && rm pycharm.tar.gz
