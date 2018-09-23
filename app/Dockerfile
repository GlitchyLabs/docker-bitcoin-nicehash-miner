FROM glitchylabs/docker-bitcoin-nicehash-miner:nheqminer as builder

FROM glitchylabs/docker-bitcoin-nicehash-miner:base
LABEL maintainer="glitchylabs@gmail.com"

WORKDIR /app/

COPY --from=builder /app/nheqminer/Linux_cmake/nheqminer_cpu_tromp/nheqminer_cpu_tromp .
COPY script/ .

CMD ["/bin/bash", "start.sh"]
