ARG ARCH
FROM ${ARCH}alpine:3
ARG TARGETPLATFORM
ARG BUILDPLATFORM
ENV TARGETPATH=${TARGETPLATFORM:-"."}
COPY package/deploy.sh /usr/bin/
COPY bin/$TARGETPATH/log-aggregator /usr/bin/
CMD ["deploy.sh"]
