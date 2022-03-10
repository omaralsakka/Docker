FROM	debian

RUN		apt-get update -y && apt-get upgrade -y && \
		apt install git -y && apt install -y git build-essential vim sudo ufw net-tools

RUN		sudo apt-get update
RUN		sudo apt-get install -y ca-certificates curl gnupg lsb-release
RUN		curl -fsSL https://download.docker.com/linux/debian/gpg | \
		sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
RUN		echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/debian \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
RUN		sudo apt-get update && sudo apt-get install -y docker-ce docker-ce-cli containerd.io
RUN		sudo apt-get install -y python3.6
RUN		sudo apt-get update -y && sudo apt-get upgrade -y 