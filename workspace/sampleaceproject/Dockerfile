FROM ibmcom/ace:latest

ARG PROJECT
ENV PROJECT=$PROJECT
RUN echo $PROJECT
RUN mkdir -p /home/aceuser/bars
RUN ls -la
RUN cp workspace/$PROJECT/gen/*.bar /home/aceuser/bars
RUN chown aceuser:aceuser /home/aceuser/bars
RUN ace_compile_bars.sh
