FROM alpine

RUN apk --no-cache add tor bash shadow

RUN mkdir -p /var/lib/tor \
 && chown -R tor /var/lib/tor \
 && chmod 1777 /var/lib/tor

ADD run.sh /run.sh

EXPOSE 9050

VOLUME /var/lib/tor

CMD /run.sh
