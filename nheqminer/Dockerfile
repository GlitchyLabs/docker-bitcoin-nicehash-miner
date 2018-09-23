FROM glitchylabs/docker-bitcoin-nicehash-miner:base
LABEL maintainer="glitchylabs@gmail.com"

RUN git clone -b Linux https://github.com/nicehash/nheqminer.git --depth=1

RUN cd nheqminer/Linux_cmake/nheqminer_cpu_tromp \
    && cmake . \
    && make -j $(nproc)
