<div align="center">
    <h1><code>🏛️</code> Boilerplate</h1>
    <p style="font-style: italic;">A template for creating new projects.</p>
</div>

## `📖` About

This is a template for creating new projects. It includes a **[Docker compose](https://docs.docker.com/compose/)** file for running a development environment, a **[Kubernetes](https://kubernetes.io/)** with **[Helm](https://helm.sh)** chart for deploying to a cluster.

## `🚀` Quickstart

```bash
🏠
├── docker-compose 🦑
│  ├── cadvisor
│  │  └── docker-compose.yml
│  ├── grafana
│  │  └── docker-compose.yml
│  ├── nginxproxymanager
│  │  └── docker-compose.yml
│  ├── nodeexporter
│  │  └── docker-compose.yml
│  ├── portainer
│  │  └── docker-compose.yml
│  ├── portainer-agent
│  │  └── docker-compose.yml
│  ├── prometheus
│  │  ├── config
│  │  │  └── prometheus.yml
│  │  └── docker-compose.yml
│  ├── teleport
│  │  ├── config
│  │  │  └── teleport.yaml
│  │  └── docker-compose.yml
│  ├── traefik
│  │  ├── config
│  │  │  └── traefik.yml
│  │  └── docker-compose.yml
│  └── uptimekuma
│     └── docker-compose.yml
└── kubernetes ☸️
   ├── cert-manager
   │  ├── README.md
   │  └── templates
   │     ├── certificate.yml
   │     ├── clusterissuer-acme.yml
   │     ├── clusterissuer-selfsigned.yml
   │     └── secret-cloudflare.yml
   ├── portainer
   │  ├── README.md
   │  └── templates
   │     └── portainer-ingress.yml
   └── traefik
      ├── README.md
      ├── templates
      │  ├── cloudflare-secret.yml
      │  ├── ingress.yml
      │  └── ingressroutetcp.yml
      └── values.yml
```

## `©️` References

- [Christain Lempa](https://github.com/ChristianLempa/boilerplates/) 🧔 Heavily inspired by this repository and learned a lot from it.
- [Docker](https://www.docker.com/) 🌐 Containerization platform.
- [Docker Compose](https://docs.docker.com/compose/) 🌐 Tool for defining and running multi-container Docker applications.
- [Kubernetes](https://kubernetes.io/) 🌐 Container orchestration platform.
- [Helm](https://helm.sh) 🌐 Package manager for Kubernetes.

## `📝` License

Licensed under the [MIT License](./LICENSE).
