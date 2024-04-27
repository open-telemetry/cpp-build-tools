ARG BUILDIFIER_VERSION=3.5.0
ARG CLANG_VERSION=18
ARG CMAKE_FORMAT_VERSION=0.6.13

FROM ubuntu:24.04
LABEL maintainer="The OpenTelemetry Authors"
RUN apt update

ARG CLANG_VERSION
RUN apt install -y clang-format-${CLANG_VERSION} python3 python3-pip git curl \
    && ln /usr/bin/clang-format-${CLANG_VERSION} /usr/bin/clang-format

ARG CMAKE_FORMAT_VERSION
RUN pip3 install --break-system-packages cmake_format==${CMAKE_FORMAT_VERSION}

ARG BUILDIFIER_VERSION
RUN curl -L -o /usr/local/bin/buildifier https://github.com/bazelbuild/buildtools/releases/download/${BUILDIFIER_VERSION}/buildifier
RUN chmod +x /usr/local/bin/buildifier

COPY format.sh /
ENTRYPOINT ["bash", "/format.sh"]
