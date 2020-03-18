import InstallMac from "../../src/components/InstallMac"
import InstallLinux from "../../src/components/InstallLinux"
import InstallWindows from "../../src/components/InstallWindows"
import InstallEdgectl from "../../src/components/InstallEdgectl"
import InstallTLS from "../../src/components/InstallTLS"
import InstallMinikube from "../../src/components/InstallMinikube"

---
   description: In this guide, we'll walk through the process of deploying Ambassador Edge Stack in Kubernetes for ingress routing.
---
# Quick Start Installation Guide

In just four minutes, your cluster will be routing HTTPS requests from the
Internet to a backend service.

The Ambassador Edge Stack is deployed to Kubernetes via YAML for MacOS, Linux, and
Windows. For other options, such as Docker, click [here](/user-guide/install).

<InstallMac></InstallMac>
 
<InstallLinux></InstallLinux>
 
<InstallWindows></InstallWindows>

## Installation

Your terminal will print something similar to the following as it provisions a load balancer, configures TLS, and provides you with an `edgestack.me` subdomain:

<InstallEdgectl></InstallEdgectl>

Provide an email address as required by the ACME TLS certificate provider, Let's
Encrypt. Then your terminal will print something similar to the following:

<InstallTLS></InstallTLS>

The `random-word-1234.edgestack.me` is a provided subdomain that allows the
Ambassador Edge Stack to automatically provision TLS and HTTPS for a domain
name, so you can get started right away.

Your new [Edge Policy Console](/about/edge-policy-console) will open
automatically in your browser at the provided URL or IP address. **Note that the provided `random-word.edgestack.me` domain name will expire after 90 days**.

![AES success](/../../doc-images/aes-success.png)

### Minikube

Minikube users will see something similar to the following:

<InstallMinikube></InstallMinikube>

## Installation Success

Congratulations, you've installed the Ambassador Edge Stack! Take advantage of
the quick start demo by [creating a mapping](/user-guide/quickstart-demo) on
your cluster using the Ambassador Edge Stack.

### What’s Next?

The Ambassador Edge Stack has a comprehensive range of [features](/features/) to
support the requirements of any edge microservice. To learn more about how the
Ambassador Edge Stack works, along with use cases, best practices, and more,
check out the [Welcome page](/docs/) or read the [Ambassador
Story](/about/why-ambassador).

For a custom configuration, you can install the Ambassador Edge Stack [manually](/user-guide/manual-install).
