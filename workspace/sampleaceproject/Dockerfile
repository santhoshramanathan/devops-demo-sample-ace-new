#FROM cp.icr.io/cp/appc/ace-server-prod@sha256:8df2fc5e76aa715e2b60a57920202cd000748476558598141a736c1b0eb1f1a3
FROM default-route-openshift-image-registry.cloud-integration-ocp45-6fb0b86391cd68c8282858623a1dddff-0000.eu-gb.containers.appdomain.cloud/aceistio3/aceimage-prod-10:latest
#COPY HTTPGetApp_v2.bar /home/aceuser/initial-config/bars/
#RUN ace_compile_bars.sh
USER root

COPY HTTPGetApp_v2.bar /home/aceuser/bars
RUN  chmod -R ugo+rwx /home/aceuser

USER aceuser

RUN ace_compile_bars.sh

USER root

RUN  chmod -R ugo+rwx /home/aceuser

USER aceuser
