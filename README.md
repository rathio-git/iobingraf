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


Install Node.js first
<pre><code>curl -sLf https://deb.nodesource.com/setup_12.x | sudo -E bash -
</code></pre>
<pre><code>sudo apt-get install -y nodejs
</code></pre>
now install Iobroker
<pre><code>curl -sLf https://iobroker.net/install.sh | bash -
</code></pre>

# 2. install Docker with docker-compose 

install docker
<pre><code>curl -sSL https://get.docker.com | sh
</code></pre>

install docker-compose
<pre><code>sudo apt install libffi-dev libssl-dev -y
sudo apt install python3-dev -y
sudo apt install python3 python3-pip -y
</code></pre>


<pre><code>
</code></pre>
