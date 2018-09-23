FROM glitchylabs/docker-bitcoin-nicehash-miner:base
LABEL maintainer="glitchylabs@gmail.com"

WORKDIR /app/

COPY cpuminer .
COPY script/ .

CMD ["/bin/bash", "start.sh"]
