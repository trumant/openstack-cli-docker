# openstack-cli-docker

This is an Ansible-Container project for producing a Docker container containing all of the
OpenStack CLI tools for a specific version of OpenStack.

## Requirements

 * Docker
 * Ansible 2.1.1.0
 * Ansible-Container

## Getting Started

To build a container image with all of the OpenStack Newton version CLI tools:

```shell
ansible-container build --from-scratch
```

This will produce an image named: openstack-cli-docker-os_cli_newton

To build a container image with the Mitaka version of the CLI tools, specify the version like:

```shell
AC_OPENSTACK_VERSION="mitaka" ansible-container build --from-scratch
```

## Using the CLI Container

```shell
./os_cli newton
```