# ansible-ntp
Deploy docker container with NTP-server based on cturra/ntp (https://hub.docker.com/)

## Role variables

| Variable | Default value | Description |
| :---:        |     :---:      |         :---: |
| ntp_service_name   | ntp-docker      | Service name in OS   |
| uninstall_service     | false       | Uninstallation marker      |
| ntp_host_port     | 123       | Host network port      |
| ntp_container_port     | 123       | Container network port      |
| port_type     | udp       | Type of port (tcp/udp)      |
| global_ntp_servers     | 162.159.200.1      | Global NTP-server IP      |
| docker_image     | cturra/ntp       | Docker image (https://hub.docker.com/)      |

### How to use
    - installation: just start the role
    - uninstallation: add --extra-vars "uninstall_service=true"
