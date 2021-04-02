# unifi-systemd

Systemd Service for UniFi OS

## Installation

``` sh
podman exec unifi-os sh -c "curl -fsSLo /tmp/unifi-systemd_1.0.0_all.deb https://github.com/ntkme/unifi-systemd/releases/download/v1.0.0/unifi-systemd_1.0.0_all.deb && dpkg -i /tmp/unifi-systemd_1.0.0_all.deb && rm /tmp/unifi-systemd_1.0.0_all.deb"
```

## Uninstallation

``` sh
podman exec unifi-os sh -c "dpkg -P unifi-systemd"
```

## Usage

Put `systemd` units in `/mnt/data/etc/systemd/system`, which will be loaded by `unifi-systemd` container.
