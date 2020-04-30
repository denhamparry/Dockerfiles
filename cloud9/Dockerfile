FROM linuxserver/cloud9:latest

ARG BUILD_DATE
ARG VERSION
LABEL build_version="DenhamParry version:- ${VERSION} Build-date:- ${BUILD_DATE}"
LABEL maintainer="denhamparry"

RUN \
  echo " ***** Add default content *****" &&\
   mkdir "/build" &&\
  echo "DenhamParry version:- ${VERSION} Build-date:- ${BUILD_DATE}" >> /build/version.txt
