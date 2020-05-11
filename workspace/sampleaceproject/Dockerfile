FROM ibmcom/ace:latest

ARG PROJECT1
ENV PROJECT=$PROJECT1
RUN echo $PROJECT
RUN mkdir -p /home/aceuser/bars
RUN ls -la /
COPY workspace/sampleaceproject/gen/*.bar /home/aceuser/bars
RUN chown aceuser:aceuser /home/aceuser/bars
RUN ace_compile_bars.sh
