FROM ibmcom/ace:latest

ARG PROJECT1
RUN mkdir -p /home/aceuser/bars
COPY $PROJECT1 /home/aceuser/bars
RUN chown aceuser:aceuser /home/aceuser/bars
RUN ace_compile_bars.sh
