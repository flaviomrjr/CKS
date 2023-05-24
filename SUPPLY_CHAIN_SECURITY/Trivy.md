TRIVY
=====

trivy image --severity CRITICAL nginx:1.18.0

trivy image --severity CRITICAL, HIGH nginx:1.18.0

trivy image --ignore-unfixed nginx:1.18.0

docker save nginx:1.18.0 > nginx.tart

trivy image --input nginx.tar