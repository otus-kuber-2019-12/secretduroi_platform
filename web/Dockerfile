FROM python:3

# Create app directory
WORKDIR /app

# Bundle app source
COPY ./app /app

RUN groupadd -g 1001 app && \
    useradd -r -u 1001 -g app app
USER app

EXPOSE 8000
CMD [ "python3", "-m", "http.server", "8000" ]
