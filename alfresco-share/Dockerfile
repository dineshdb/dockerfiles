FROM docker.io/alfresco/alfresco-share:7.2.0
ENV TOMCAT_DIR=/usr/local/tomcat
# Patch for https://github.com/Alfresco/acs-community-packaging/issues/367
RUN sed -i 's@<show-authorization-status>true</show-authorization-status>@<show-authorization-status>false</show-authorization-status>@' \
	$TOMCAT_DIR/shared/classes/alfresco/web-extension/share-config-custom.xml
