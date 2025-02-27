ARG VARIANT="12.5.1-cudnn-runtime-ubuntu22.04"

FROM nvidia/cuda:${VARIANT}

RUN apt-get update && apt-get install -y \
    curl \
    git \
    && apt-get upgrade -y \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN curl -LsSf https://astral.sh/uv/0.6.3/install.sh | sh 

WORKDIR /workspace
