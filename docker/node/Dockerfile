FROM node:24

ARG USER_ID=1000
ARG GROUP_ID=1000

RUN groupmod -g ${GROUP_ID} node || true && \
    usermod -u ${USER_ID} node || true

WORKDIR /app
USER node

CMD ["tail", "-f", "/dev/null"]
