# A Data Volume Container to persist the expensively built virtualenv across
# rebuilds of the "dev" image

# Same base as dev image, to save space. (It's copy-on-write.)
FROM ubuntu@sha256:e6173d4dc55e76b87c4af8db8821b1feae4146dd47341e4d431118c7dd060a74

# Match UID with dev image:
RUN mkdir /venv && chown -R 1000:1000 /venv
VOLUME /venv
