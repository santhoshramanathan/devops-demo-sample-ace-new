FROM ibmcom/ace:latest

ENV PROJECT=$PROJECT
RUN mkdir -p /home/aceuser/bars
COPY workspace/$PROJECT/gen/*.bar /home/aceuser/bars
RUN chown aceuser:aceuser /home/aceuser/bars
RUN ace_compile_bars.sh
