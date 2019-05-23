ARG IMAGE_BASE

FROM $IMAGE_BASE
# Note: Latest version of kubectl may be found at:
# https://aur.archlinux.org/packages/kubectl-bin/
ARG KUBE_LATEST_VERSION="v1.14.1"
# Note: Latest version of helm may be found at:
# https://github.com/kubernetes/helm/releases
ARG HELM_VERSION="v2.14.0"

RUN apk add --no-cache ca-certificates bash git openssh curl

RUN wget -q https://storage.googleapis.com/kubernetes-release/release/$KUBE_LATEST_VERSION/bin/linux/amd64/kubectl -O /usr/local/bin/kubectl \
    && chmod +x /usr/local/bin/kubectl \
    && wget -q https://storage.googleapis.com/kubernetes-helm/helm-$HELM_VERSION-linux-amd64.tar.gz -O - | tar -xzO linux-amd64/helm > /usr/local/bin/helm \
    && chmod +x /usr/local/bin/helm
