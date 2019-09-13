FROM python:3.4-slim

RUN pip install snmpsim

RUN mkdir /data

RUN mkdir /cache

CMD snmpsimd.py --agent-udpv4-endpoint=0.0.0.0:161 --v2c-arch --process-user=root --process-group=root --cache-dir=/cache  --data-dir=/data $EXTRA_FLAGS
#CMD snmpsimd.py --agent-udpv4-endpoint=0.0.0.0:161 --process-user=nobody --process-group=nogroup --cache-dir=/cache --data-dir=/data $EXTRA_FLAGS
# --process-user=simulator --process-group=simulator --data-dir=$HOME $EXTRA_FLAGS
