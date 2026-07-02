# VIGL

<img width="401" height="351" alt="image" src="https://github.com/user-attachments/assets/bf8609f2-eb7b-490c-be3e-ed4a4afe33bd" />



VIGL is a small progressive web application (PWA) that starts a wake lock to prevent the device from going to sleep or shutting off the display. This is intended to be run in a Docker container behind a TLS reverse proxy such as Traefik.

Run this in a container with `compose.yml`

```
services:
    vigl:
      image: ghcr.io/c360e5f1/vigl:latest
      ports:
        - "8080:8080"
      restart: unless-stopped
```

***

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see http://www.gnu.org/licenses/.
