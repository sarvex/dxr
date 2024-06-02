# A Data Volume Container to persist some source code to index across rebuilds
# of the "dev" image

# Same base as dev image, to save space. (It's copy-on-write.)
FROM ubuntu@sha256:3f85b7caad41a95462cf5b787d8a04604c8262cdcdf9a472b8c52ef83375fe15

# Match UID with dev image:
RUN mkdir /code && chown -R 1000:1000 /code
VOLUME /code
