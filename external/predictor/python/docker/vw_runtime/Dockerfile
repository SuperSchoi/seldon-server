FROM seldonio/vw_train

ENV HOME /root
ENV DEBIAN_FRONTEND noninteractive

RUN \
    apt-get update && \
    apt-get -y -q install telnet procps

RUN pip install Flask gunicorn

ADD ./scripts /vw/vw_runtime

# Define default command.
CMD ["bash"]
