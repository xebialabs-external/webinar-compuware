FROM mdns/sshd:latest

RUN apt-get update && apt-get install -y git && rm -rf /var/lib/apt/lists/*

COPY TotalTestCLI.sh /usr/local/bin/topazcli/
COPY *.txt /usr/local/bin/topazcli/