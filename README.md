This container helps resolve an issue with Container Optimized OS.  The OS does not come with docker-compose, and instead expects users to use containerized docker-compose.  However the official containerized docker-compose does not include docker-credential-gcr, which is needed to pull Docker images from a private Google Container Registry.

This container uses the official docker-compose as a base, and adds docker-credential-gcr.  It can be used just like the normal containerized docker-compose, but can now access gcr.io.

Images should be available at `ghcr.io/fpgaminer/docker-compose-gcr:latest`; updated monthly.