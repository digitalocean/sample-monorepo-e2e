FROM scratch as init
ADD . /app/

FROM alpine:3.23
RUN mkdir /app
COPY --from=init /app/ok /app/
COPY ./another-file /app/
WORKDIR /app
