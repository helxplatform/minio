# MINIO deployment on Kubernetes.

## This repo built from the official Helm Charts except with a few changes to the persistence storage.

The following values are required.
https://github.com/helxplatform/minio/blob/e099c5beb1774e37d79e5f8a1dfc8383d6b1438b/values.yaml#L111-L133

The default SecretKey and AccessKey are set to minio123 and minio respectively.
https://github.com/helxplatform/minio/blob/e099c5beb1774e37d79e5f8a1dfc8383d6b1438b/values.yaml#L65-L66

To run minio - make sure you are using helm3,
```helm install minio minio/ -n <namespace>```
