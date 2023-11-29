FROM mcr.microsoft.com/devcontainers/python:0-3.11
# trunk-ignore(hadolint/DL4006)
# RUN wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | apt-key add -
# RUN sh -c 'echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list'
# ENV CHROME_VERSION="114.0.5735.90"
# RUN apt-get -y update
# RUN apt-get install -y wget git
# RUN wget -q "https://dl.google.com/linux/chrome/deb/pool/main/g/google-chrome-stable/google-chrome-stable_${CHROME_VERSION}-1_amd64.deb" ;sudo dpkg -i "google-chrome-stable_${CHROME_VERSION}-1_amd64.deb"; rm "google-chrome-stable_${CHROME_VERSION}-1_amd64.deb"
# RUN apt --fix-broken install -y

# install chromedriver
# RUN apt-get install -y unzip
# RUN wget -O /tmp/chromedriver.zip http://chromedriver.storage.googleapis.com/${CHROME_VERSION}/chromedriver_linux64.zip
# RUN unzip /tmp/chromedriver.zip chromedriver -d /usr/local/bin/
# RUN apt-get clean
# set display port to avoid crash
# ENV DISPLAY=:99
WORKDIR /app
COPY .. /app
# RUN pip install -r /app/requirements.txt
# CMD python /app/main.py