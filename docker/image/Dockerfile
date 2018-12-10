FROM library/nginx

ARG ARTIFACT_ID
ARG BUILD_DATE
ARG VCS_URL
ARG VCS_REF
ARG VENDOR
ARG VERSION
ARG SCHEMA_VERSION

LABEL org.label-schema.build-date="${BUILD_DATE}"
LABEL org.label-schema.vcs-url="${VCS_URL}"
LABEL org.label-schema.vcs-ref="${VCS_REF}"
LABEL org.label-schema.vendor="${VENDOR}"
LABEL org.label-schema.version="${VERSION}"
LABEL org.label-schema.schema-version="${SCHEMA_VERSION}"
LABEL org.label-schema.name="${ARTIFACT_ID}"

COPY container/ /