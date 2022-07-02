# Copyright (c) 2022 Paul Barker
# SPDX-License-Identifier: Apache-2.0

ARG BASE_IMAGE=ghcr.io/unnecessary-abstraction/yacron:latest
FROM ${BASE_IMAGE}

RUN apk add --update-cache git rclone build-base libffi-dev python3-dev && \
    rm -rf /var/cache/apk/* && \
    python3 -m pip install --no-cache-dir mirrorshades PyGithub python-gitlab
