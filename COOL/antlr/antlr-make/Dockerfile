FROM anapsix/alpine-java:8_jdk_unlimited

MAINTAINER Goutham Veeramachaneni <cs14btech11014@iith.ac.in>

WORKDIR /antlr

ADD antlr-4.5.3-complete.jar .

ENV CLASSPATH ".:/antlr/antlr-4.5.3-complete.jar:$CLASSPATH"

# To load aliases
ENV ENV /root/.profile
RUN echo 'alias antlr4="java -jar /antlr/antlr-4.5.3-complete.jar"' >> /root/.profile
RUN echo 'alias grun="java org.antlr.v4.gui.TestRig"' >> /root/.profile


RUN apk add --no-cache make
