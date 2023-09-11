FROM python:3.9 AS stage1

WORKDIR /app

RUN git clone https://github.com/ssingh-1728/docker

WORKDIR /app/docker/distroless-multi-stage/

FROM python:3.9-slim AS final

COPY --from=stage1 /app/docker/distroless-multi-stage/ /app/

WORKDIR /app

ENTRYPOINT ["python3", "app.py"]
