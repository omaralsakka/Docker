FROM	ruby:2.7
RUN		apt-get update && \
		apt-get upgrade -y && \
		apt-get install -y sqlite3 nodejs npm

ONBUILD WORKDIR	/opt/app
ONBUILD ADD		sample_app /opt/app

ONBUILD RUN		bundle install --without 'production'
ONBUILD RUN		npm install --global yarn
ONBUILD RUN		yarn install
ONBUILD RUN		rails db:migrate