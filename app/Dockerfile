FROM glitchylabs/docker-bitcoin-nicehash-miner:base:nheqminer as builder

FROM glitchylabs/docker-bitcoin-nicehash-miner:base
LABEL maintainer="glitchylabs@gmail.com"

WORKDIR /app/

COPY --from=builder /app/nheqminer/Linux_cmake/nheqminer_cpu/nheqminer_cpu .
COPY script/ .

CMD ["/bin/bash", "start.sh"]
