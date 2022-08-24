FROM gcr.io/google.com/cloudsdktool/google-cloud-cli:399.0.0-alpine as build
ENV USE_GKE_GCLOUD_AUTH_PLUGIN=True
RUN gcloud components install \
        kubectl \
        gke-gcloud-auth-plugin \
    && rm -rf $(find google-cloud-sdk/ -regex ".*/__pycache__") \
    && rm -rf google-cloud-sdk/.install/.backup
