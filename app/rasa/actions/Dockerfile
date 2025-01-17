FROM rasa/rasa:latest

COPY . /app

WORKDIR /app

USER root
RUN pip install python-dotenv rasa-sdk requests
USER 1001

EXPOSE 5055

CMD ["run", "actions", "--debug"]
