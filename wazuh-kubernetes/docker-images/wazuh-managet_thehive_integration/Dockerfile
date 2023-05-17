FROM wazuh/wazuh-manager:4.4.1
RUN /var/ossec/framework/python/bin/pip3 install thehive4py==1.8.1
COPY ./custom-w2thive /var/ossec/integrations/
COPY ./custom-w2thive.py /var/ossec/integrations/
RUN chmod 777 /var/ossec/integrations/custom-w2thive.py
RUN chmod 777 /var/ossec/integrations/custom-w2thive

ENTRYPOINT [ "/init" ]