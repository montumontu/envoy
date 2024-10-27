FROM envoyproxy/envoy:v1.21-latest

ENV AWS_ACCESS_KEY_ID=
ENV AWS_SECRET_ACCESS_KEY=
ENV AWS_REGION=us-east-1
ENV aws_session_token=
ENV AWS_SESSION_TOKEN=


WORKDIR /etc/envoy

COPY ./envoy.yaml ./envoy.yaml

EXPOSE 10000

CMD ["envoy", "-c",  "/etc/envoy/envoy.yaml", "--log-level", "debug"]
