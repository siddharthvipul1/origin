FROM openshift/origin-source

RUN INSTALL_PKGS="origin-service-catalog" && \
    yum install -y ${INSTALL_PKGS} && \
    rpm -V ${INSTALL_PKGS} && \
    yum clean all

CMD [ "/usr/bin/controller-manager" ]
