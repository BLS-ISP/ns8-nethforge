# BLS-ISP NethServer 8 Software Repository

This repository provides the NethServer 8 (NS8) Software Center index for modules published by **BLS-ISP**.

## Available Modules

- **[Vaultwarden](https://github.com/BLS-ISP/NS8-Vaultwarden)** (`ghcr.io/bls-isp/vaultwarden`) — Self-hosted, Bitwarden-compatible password manager server with Admin Panel, NS8 Smarthost integration, LDAP/AD user invitation sync, Mobile Push Notifications, and automated online SQLite backup/restore.
- **[GitLab CE](https://github.com/BLS-ISP/NS8-GitLab)** (`ghcr.io/bls-isp/gitlab`) — Self-hosted GitLab Community Edition DevSecOps platform for Git repositories, CI/CD (with auto-registered rootless Podman Runner), Container Registry, NS8 LDAP/AD authentication, Smarthost integration, and Git over SSH.
- **[VPN Portal](https://github.com/BLS-ISP/ns8-vpnportal)** (`ghcr.io/bls-isp/vpn`) — Business Roadwarrior & Site-to-Site VPN combining WireGuard and IPv4/IPv6 DS-Lite OpenVPN TCP fallback with live NS8 Active Directory / OpenLDAP user lifecycle sync, Traefik TOTP 2FA Self-Service Portal, and compliance Audit Logging.
- **[Mail Toolbox](https://github.com/BLS-ISP/ns8-mailtoolbox)** (`ghcr.io/bls-isp/mail-toolbox`) — Delegated secretariat Out-of-Office & forwarding portal (with non-destructive SOGo coexistence), central Before-DKIM dynamic AD/LDAP company signatures, daily spam quarantine digest with scanner-safe release, Rspamd mail-tracking search, and external POP3/IMAP connectors.
- **[SoftwareManager](https://github.com/BLS-ISP/ns8-softwaremanager)** (`ghcr.io/bls-isp/softwaremanager`) — Central cross-platform endpoint, OS patch (Windows WUA & Linux APT/DNF), and self-service Software Center manager for Windows and Linux workstations and servers with Ed25519-signed deployments, custom SHA-256 package repository, maintenance windows, and NS8 AD/LDAP authentication.

## How to add this repository in NethServer 8

In the NethServer 8 Cluster Admin UI, navigate to **Settings → Software repositories → Add repository**:

- **Name:** `bls-isp`
- **URL:**
  ```text
  https://raw.githubusercontent.com/BLS-ISP/ns8-nethforge/repomd/ns8/updates/
  ```

Repository metadata (`repodata.json`) is rebuilt automatically every 6 hours (`00:25`, `06:25`, `12:25`, `18:25` UTC) and on every push to `main`.
