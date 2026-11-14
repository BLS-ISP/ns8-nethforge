# BLS-ISP NethServer 8 Software Repository

This repository provides the NethServer 8 (NS8) Software Center index for modules published by **BLS-ISP**.

## Available Modules

- **[Vaultwarden](https://github.com/BLS-ISP/NS8-Vaultwarden)** (`ghcr.io/bls-isp/vaultwarden`) — Self-hosted, Bitwarden-compatible password manager server with Admin Panel, NS8 Smarthost integration, LDAP/AD user invitation sync, Mobile Push Notifications, and automated online SQLite backup/restore.
- **[GitLab CE](https://github.com/BLS-ISP/NS8-GitLab)** (`ghcr.io/bls-isp/gitlab`) — Self-hosted GitLab Community Edition DevSecOps platform for Git repositories, CI/CD (with auto-registered rootless Podman Runner), Container Registry, NS8 LDAP/AD authentication, Smarthost integration, and Git over SSH.

## How to add this repository in NethServer 8

In the NethServer 8 Cluster Admin UI, navigate to **Settings → Software repositories → Add repository**:

- **Name:** `bls-isp`
- **URL:**
  ```text
  https://raw.githubusercontent.com/BLS-ISP/ns8-nethforge/repomd/ns8/updates/
  ```

Repository metadata (`repodata.json`) is rebuilt automatically every 6 hours (`00:25`, `06:25`, `12:25`, `18:25` UTC) and on every push to `main`.
