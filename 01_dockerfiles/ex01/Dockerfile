FROM		debian
ENV			TS3SERVER_LICENSE=accept
RUN			apt-get update -y && apt-get upgrade -y && \
			apt-get install -y wget bzip2 && \
			wget https://files.teamspeak-services.com/releases/server/3.13.6/teamspeak3-server_linux_amd64-3.13.6.tar.bz2 && \
			tar xfvj teamspeak3-server_linux_amd64-3.13.6.tar.bz2 && \
			rm teamspeak3-server_linux_amd64-3.13.6.tar.bz2
WORKDIR		teamspeak3-server_linux_amd64
ENTRYPOINT	sh ts3server_minimal_runscript.sh
