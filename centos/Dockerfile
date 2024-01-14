FROM centos:latest
LABEL maintainer="Lorenz Egginger 'lorenz@example.com'"
ENV REFRESHED_AT 2024-01-14
# hadolint ignore=DL3032,DL3033
RUN yum -y install ruby rubygems rubygem-rake
# hadolint ignore=DL3028,DL3059
RUN gem install --no-document rspec ci_reporter_rspec
