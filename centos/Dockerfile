# hadolint ignore=DL3007
FROM centos:latest
LABEL maintainer="Lorenz Egginger 'lorenz@example.com'"
ENV REFRESHED_AT 2024-01-14
# hadolint ignore=DL3003
RUN cd /etc/yum.repos.d/ || exit
RUN sed -i 's/mirrorlist/#mirrorlist/g' /etc/yum.repos.d/CentOS-*
# hadolint ignore=DL3059
RUN sed -i 's|#baseurl=http://mirror.centos.org|baseurl=http://vault.centos.org|g' /etc/yum.repos.d/CentOS-*
# hadolint ignore=DL3032,DL3033,DL3059
RUN yum -y install ruby rubygems rubygem-rake
# hadolint ignore=DL3028,DL3059
RUN gem install --no-document rspec ci_reporter_rspec
