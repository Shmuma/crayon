FROM tensorflow/tensorflow:latest
RUN pip install flask
ADD startup.sh /
ADD server.py /
ADD patch_tensorboard.py /
EXPOSE 5999
# TODO: move from cmd to entrypoint
ENTRYPOINT ["/bin/bash", "/startup.sh"]
