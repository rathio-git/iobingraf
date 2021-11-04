# IoBroker with InfluxDB and Grafana

This is a howto for installing Iobroker on debian or derivate.

I will install Iobroker native on the system because, i don't find
a docker container for the Raspberry Pi 4.
This howto is also for normal x86 maschines.

For InfluxDB and Grafana i provide here an docker-compose file.
so it will be very easy to install all stuff.


# 1. Step - Install Iobroker

install all last updates
<pre><code>sudo apt update && sudo apt dist-upgrade -y
</code></pre>


install Node.js first
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

install python3 and pip
<pre><code>sudo apt install libffi-dev libssl-dev -y
sudo apt install python3-dev -y
sudo apt install python3 python3-pip -y
</code></pre>

now install docker-compose
<pre><code>sudo pip3 install docker-compose
</code></pre>
This take some time, on a raspberry, please wait so long.

# 3. enable docker system service to start container on boot
<pre><code>sudo systemctl enable docker
</code></pre>


