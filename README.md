# io_influx_grafa

Iobroker and Docker with Influxdb and Grafana

This is an HowTo for install Iobroker on Debian and derivate

I will install Iobroker direct on the System because, i do not find
a Docker container for the Raspberry Pi.

For InfluxDB and Grafana i provide here an docker-compose file.
so it will be very easy to install al stuff.


# 1. Step - Install Iobroker

Install all last updates
<pre><code>sudo apt update && sudo apt dist-upgrade -y
</code></pre>


- Install Node.js first
curl -sLf https://deb.nodesource.com/setup_12.x | sudo -E bash -
sudo apt-get install -y nodejs

- now install Iobroker
curl -sLf https://iobroker.net/install.sh | bash -


# 2. install Docker with docker-compose 

- install docker
curl -sSL https://get.docker.com | sh

- install docker-compose
sudo apt-get install libffi-dev libssl-dev
sudo apt install python3-dev
sudo apt-get install -y python3 python3-pip

<pre><code>
</code></pre>
