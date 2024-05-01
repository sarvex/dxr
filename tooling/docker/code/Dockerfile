# A Data Volume Container to persist some source code to index across rebuilds
# of the "dev" image

# Same base as dev image, to save space. (It's copy-on-write.)
FROM ubuntu@sha256:562456a05a0dbd62a671c1854868862a4687bf979a96d48ae8e766642cd911e8

# Match UID with dev image:
RUN mkdir /code && chown -R 1000:1000 /code
VOLUME /code
