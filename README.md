# Apache Chemistry OpenCMIS with Security Patch

[![Java CI](https://github.com/Soontao/OpenCMIS/actions/workflows/java.yaml/badge.svg)](https://github.com/Soontao/OpenCMIS/actions/workflows/java.yaml)

> Self Maintained OpenCMIS Distribution with security patch, based on [Apache Chemistry OpenCMIS 1.1](https://chemistry.apache.org/java/opencmis.html)

> [README of apache OpenCMIS is here](./README.Apache.txt)

## Breaking Changes

- change build and runtime to `java 17`, as a consequence, must use `tomcat 9` from now
- remove `OpenCMIS - android`
- change `ThresholdOutputStream` encryption algorithm from `AES/CTR/PKCS5Padding` to `AES/CTR/NoPadding` 
- remove web ui for in-mem server

## [License](./LICENSE)
