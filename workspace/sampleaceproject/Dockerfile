FROM ibmcom/ace:latest

ARG PROJECT
RUN echo $PROJECT
RUN mkdir -p /home/aceuser/bars
RUN ls -la /workspace/source/workspace/$PROJECT/gen/
RUN cp /workspace/source/workspace/$PROJECT/gen/*.bar /home/aceuser/bars
RUN chown aceuser:aceuser /home/aceuser/bars
RUN ace_compile_bars.sh
