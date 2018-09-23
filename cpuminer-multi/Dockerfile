FROM glitchylabs/docker-bitcoin-nicehash-miner:base
LABEL maintainer="glitchylabs@gmail.com"

RUN git clone https://github.com/GeekCash/cpuminer-multi.git --depth=1

RUN cd cpuminer-multi \
  && ./autogen.sh \
  && ./configure CFLAGS="*-march=native*" --with-crypto --with-curl \
  && make
