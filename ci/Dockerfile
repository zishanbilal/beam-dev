#
# Oracle Java 8 Dockerfile
#
# https://github.com/zishanbilal/beam-dev
# https://github.com/zishanbilal/beam-dev/tree/master/ci
#

# Pull base image.
FROM ubuntu

# Install Java.
RUN \
  echo oracle-java8-installer shared/accepted-oracle-license-v1-1 select true | debconf-set-selections && \
  apt-get install -y software-properties-common && \
  add-apt-repository -y ppa:webupd8team/java && \
  curl -s https://packagecloud.io/install/repositories/github/git-lfs/script.deb.sh | bash && \
  apt-get update && \
  apt-get install -y git-lfs=2.3.4 && \
  apt-get install -y oracle-java8-installer && \
  rm -rf /var/lib/apt/lists/* && \
  rm -rf /var/cache/oracle-jdk8-installer


# Define working directory.
WORKDIR /data

# Define commonly used JAVA_HOME variable
ENV JAVA_HOME /usr/lib/jvm/java-8-oracle

# Define default command.
CMD ["bash"]
