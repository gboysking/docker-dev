FROM	ubuntu:18.04
RUN apt-get update && yes | apt-get upgrade \
&& apt-get install -y -- no-install-recommends build-essential openssh-server xauth \
&& rm -rf /var/lib/apt/lists/* \
&& sed -i "s/^.*PasswordAuthentication.*$/PasswordAuthentication yes/" /etc/ssh/sshd_config \
&& sed -i "s/^.*X11Forwarding.*$/X11Forwarding yes/" /etc/ssh/sshd_config \
&& sed -i "s/^.*X11UseLocalhost.*$/X11UseLocalhost no/" /etc/ssh/sshd_config \
&& grep "^X11UseLocalhost" /etc/ssh/sshd_config || echo "X11UseLocalhost no" >> /etc/ssh/sshd_

WORKDIR /root/


