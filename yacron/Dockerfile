# Copyright (c) 2022 Paul Barker
# SPDX-License-Identifier: Apache-2.0

FROM docker.io/library/alpine:3.16

RUN apk add --update-cache python3 py3-pip py3-wheel dumb-init bash && \
    rm -rf /var/cache/apk/* && \
    python3 -m pip install --no-cache-dir yacron

ENTRYPOINT ["/usr/bin/dumb-init", "--", "/usr/bin/yacron"]
