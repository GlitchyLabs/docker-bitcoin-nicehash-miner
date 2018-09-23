FROM ubuntu:16.04
LABEL maintainer="glitchylabs@gmail.com"

WORKDIR /app/

COPY cpuminer .
COPY script/ .

CMD ["/bin/bash", "start.sh"]
