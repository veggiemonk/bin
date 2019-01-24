FROM debian:stable-slim

LABEL "name"="git"
LABEL "maintainer"="GitHub Actions <support+actions@github.com>"
LABEL "version"="1.0.0"

LABEL "com.github.actions.name"="git for GitHub Actions"
LABEL "com.github.actions.description"="Runs git in an Action"
LABEL "com.github.actions.icon"="git-merge"
LABEL "com.github.actions.color"="black"

COPY LICENSE README.md THIRD_PARTY_NOTICE.md /

COPY entrypoint.sh /entrypoint.sh

RUN apt-get update && \
    apt-get install --no-install-recommends -y \
        git && \
    apt-get clean -y && \
    rm -rf /var/lib/apt/lists/*

ENTRYPOINT ["/entrypoint.sh"]

