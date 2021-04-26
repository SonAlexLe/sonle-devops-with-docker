FROM ubuntu:18.04
COPY script.sh .
RUN apt-get -qq update && apt-get -qq install curl
CMD ./script.sh
# docker build . -t curler
# docker run -it --rm curler