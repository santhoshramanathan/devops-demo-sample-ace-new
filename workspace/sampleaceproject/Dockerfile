FROM ibmcom/ace:latest

ARG PROJECT
RUN echo $PROJECT
RUN mkdir -p /home/aceuser/bars
RUN PWD
RUN ls -la /
RUN cp /workspace/source/workspace/sampelaceproject/gen/*.bar /home/aceuser/bars
RUN chown aceuser:aceuser /home/aceuser/bars
RUN ace_compile_bars.sh
