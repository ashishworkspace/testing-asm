FROM alpine:latest

ARG ACCESS_KEY
ARG SECRET_KEY
ENV AWS_ACCESS_KEY_ID $ACCESS_KEY
ENV AWS_SECRET_ACCESS_KEY $SECRET_KEY


ENV AWS_DEFAULT_REGION=ap-south-1


RUN apk add aws-cli

CMD ["aws",  "secretsmanager",  "get-secret-value",  "--secret-id",  "mysql_cred_github"] 