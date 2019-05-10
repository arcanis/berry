FROM alpine:latest

LABEL "com.github.actions.name"="make-commit"
LABEL "com.github.actions.description"="Generates a commit with the given message"
LABEL "com.github.actions.icon"="mic"
LABEL "com.github.actions.color"="purple"

RUN apk add --no-cache bash git

ADD entrypoint.sh /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]
