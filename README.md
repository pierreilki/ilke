# ILKILABS KUBERNETES ENGINE
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4797/badge)](https://bestpractices.coreinfrastructure.org/projects/4797)
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Filkilabs%2Filke.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Filkilabs%2Filke?ref=badge_shield)

This project is aimed to provide the simplest way to install kubernetes on AMD-64 bare-metal, virtual & Cloud environments.
Currently, Ubuntu 18.04 & 20.04,  Centos 7 and Debian 10  are supported, but several other operating systems will be available soon.

Master branch is stable.

## Table of Contents

This is a list of points that will be explained in this Readme file for the IKE project :

- [What is ILKE](#what-is-ilke)
- [How to install](#how-to-install)
- [How to give feedback](#how-to-give-feedback)
- [How to contribute](#how-to-contribute)
- [Community](#community)
- [Licensing](#licensing)

## What is ILKE

ILKE is an easy-to-use, stable Kubernetes distribution (Kubernetes v1.15, 1.16, 1.17, 1.18, 1.19, 1.20, 1.21).

By its symplicity, ILKE provide a good way to deploy and manage K8S Clusters.

ILKE is based on Ansible scripts that install and configure Kubernetes components (control plane and data plane) quickly on bare-metal / VMs / Cloud Instances, as systemd services.

This distribution is also adaptive by offering the opportunity to customize your deployment and fit to your needs : 
* OS : Ubuntu-18.04/20.04-amd64 and Centos 7.X-amd64, Debian-10-amd64 
* DNS Service: CoreDNS
* Ingress Controller Traefik v2 & HA-Proxy & Nginx (Default)
* Container Runtime: Containerd (Default) & Docker
* Certificats: Self Signed PKI using OpenSSL
* Storage: OpenEBS (Jiva and HostPath).
* Monitoring: Prometheus/Grafana/node-Exporter
* CNI plugin: Kube-router, Calico (VxLAN Cross-Subnet)
* MetalLB (L2/ARP mode for external LB)
* Metrics-Server
* Kubernetes-Dashboard

![ILKE](./images/ILKE.png)

This project is currently under active development so other customizable options will be added soon.

## How to install

To deploy your K8S cluster follow these [instructions](docs/instructions.md).

## How to give feedback

Every feedback is very welcome via the
[GitHub site](https://github.com/ilkilabs/ilke)
as issues or pull (merge) requests.

You can also give use vulnerability reports by this way.
## How to contribute


See our [Code Of Conduct](https://github.com/ilkilabs/ilke/blob/master/CODE_OF_CONDUCT.md) and [CONTRIBUTING](https://github.com/ilkilabs/ilke/blob/master/docs/CONTRIBUTING.md) for more information.

## Community

Join ILKE's community for discussion and ask questions : [ILKE's Slack](http://slack.agorakube.ilkilabs.io/)

Channels :
- **#general** - For general purpose (news, events...)
- **#developpers** - For people who contribute to ILKE by developing features
- **#end-users** - For end users who want to give us feedbacks
- **#random** - As its name suggests, for random discussions :)

## Licensing

All material here is released under the [APACHE 2.0 license](./LICENSE).
All material that is not executable, including all text when not executed,
is also released under the APACHE 2.0.
In SPDX terms, everything here is licensed under APACHE 2.0;
if it's not executable, including the text when extracted from code, it's
"(APACHE 2.0)".

Lilke almost all software today, this software depends on many
other components with their own licenses.
Not all components we depend on are APACHE 2.0-licensed, but all
*required* components are FLOSS. We prevent licensing issues
using various processes (see [CONTRIBUTING](./docs/CONTRIBUTING.md)).


[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Filkilabs%2Filke.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Filkilabs%2Filke?ref=badge_large)

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://www.ilki.fr/"><img src="https://avatars.githubusercontent.com/u/43336050?v=4?s=100" width="100px;" alt=""/><br /><sub><b>pierre villard</b></sub></a><br /><a href="#infra-pierreilki" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/pierreilki/ilke/commits?author=pierreilki" title="Tests">⚠️</a> <a href="https://github.com/pierreilki/ilke/commits?author=pierreilki" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/bryanILKI"><img src="https://avatars.githubusercontent.com/u/79568169?v=4?s=100" width="100px;" alt=""/><br /><sub><b>bryanILKI</b></sub></a><br /><a href="https://github.com/pierreilki/ilke/commits?author=bryanILKI" title="Code">💻</a> <a href="https://github.com/pierreilki/ilke/commits?author=bryanILKI" title="Documentation">📖</a> <a href="#maintenance-bryanILKI" title="Maintenance">🚧</a></td>
  </tr>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!