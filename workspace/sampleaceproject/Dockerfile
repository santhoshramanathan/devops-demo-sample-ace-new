FROM default-route-openshift-image-registry.cloud-integration-ocp45-6fb0b86391cd68c8282858623a1dddff-0000.eu-gb.containers.appdomain.cloud/aceistio3/aceimage-prod-10:latest
COPY . /home/aceuser/sampleaceproject
RUN export LICENSE="accept" \
    && source /opt/ibm/ace-11/server/bin/mqsiprofile \
    && mkdir /home/aceuser/bars \
    && mqsipackagebar -a bars/sampleaceproject.bar -k sampleaceproject \
    && mqsibar -a bars/sampleaceproject.bar -w /home/aceuser/ace-server \
    && chmod -R 777 /home/aceuser/ace-server/run/sampleaceproject