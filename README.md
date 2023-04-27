# Apache Chemistry OpenCMIS with Security Patch

[![Build Status](https://travis-tools.cloud.sap.corp/I337313/OpenCMIS.svg?token=DUfaW1Ls7wxHnGZXYmEK&branch=main)](https://travis-tools.cloud.sap.corp/I337313/OpenCMIS)

> Self Maintained OpenCMIS Distribution with security patch, based on [Apache Chemistry OpenCMIS 1.1](https://chemistry.apache.org/java/opencmis.html)

> [README of apache OpenCMIS is here](./README.Apache.txt)

## Breaking Changes

- upgrade to build environment and target `jdk8`
- remove `OpenCMIS - android` and `OpenCMIS - workbench`
- upgrade java runtime to java 17
- change `ThresholdOutputStream` encryption algorithm from `AES/CTR/PKCS5Padding` to `AES/CTR/NoPadding` 

## [License](./LICENSE)
