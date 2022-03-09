FROM		debian
ENV			TS3SERVER_LICENSE=accept
RUN			apt-get update -y && apt-get upgrade -y && \
			apt-get install -y wget bzip2 && \
			wget https://files.teamspeak-services.com/releases/server/3.13.6/teamspeak3-server_linux_amd64-3.13.6.tar.bz2 && \
			tar xfvj teamspeak3-server_linux_amd64-3.13.6.tar.bz2 && \
			rm teamspeak3-server_linux_amd64-3.13.6.tar.bz2
WORKDIR		teamspeak3-server_linux_amd64
ENTRYPOINT	sh ts3server_minimal_runscript.sh

#first docker build -t omar/ex01 .
#second docker run -it --rm -p=9987:9987/udp  -p=10011:10011 -p=30033:30033 omar/ex01
#copy the token and past it in connect-teamspeak app box