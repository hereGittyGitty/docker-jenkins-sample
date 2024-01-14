FROM debian:bullseye
LABEL maintainer="Lorenz Egginger 'lorenz@example.com'"
ENV REFRESHED_AT 2024-01-14
# hadolint ignore=DL3009
RUN apt-get update
# hadolint ignore=DL3008,DL3059,DL3015
RUN apt-get -y install ruby rake
# hadolint ignore=DL3028,DL3059
RUN gem install --no-document rspec ci_reporter_rspec
