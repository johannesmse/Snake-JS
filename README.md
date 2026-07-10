https://johannes.oleherman.com

## Run offline / locally

The entire tool is self contained inside `index.html` - you can download this file and run it in your browser.

When this is deployed, it is running in a minimal nginx Dockerfile (just 2 lines).
You can run this locally as well, with `docker`:

```bash
docker build --tag snake-js . && docker run -it -p 8000:80 --name snake-js --rm snake-js
```

Or with `podman`:

```bash
podman build --tag snake-js . && podman run -it -p 8000:80 --name snake-js --rm snake-js
```

Open in the browser:

http://127.0.0.1:8000
