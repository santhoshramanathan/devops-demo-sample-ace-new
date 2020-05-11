FROM ibmcom/ace:latest

RUN mkdir -p /home/aceuser/bars
COPY workspace/sampleaceproject/gen/*.bar /home/aceuser/bars
RUN chown aceuser:aceuser /home/aceuser/bars
RUN ace_compile_bars.sh
