FROM python:3.6-slim

LABEL "com.github.actions.name"="Black Code Formatter"
LABEL "com.github.actions.description"="Format Python code using black"
LABEL "com.github.actions.icon"="code"
LABEL "com.github.actions.color"="yellow"

LABEL "repository"="https://github.com/fritzlabs/actions/black"
LABEL "homepage"="https://github.com/fritzlabs/actions/black"
LABEL "maintainer"="Jameson Toole <jameson@fritz.ai>"

RUN pip install black==20.8b1

COPY entrypoint.sh /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
