FROM alpine:latest

LABEL "com.github.actions.name"="if-path-changed"
LABEL "com.github.actions.description"="Only lets the workflow continue if a regex matches the changed files"
LABEL "com.github.actions.icon"="mic"
LABEL "com.github.actions.color"="purple"

RUN apk add --no-cache bash jq
RUN apk add --no-cache --upgrade grep

ADD entrypoint.sh /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]
