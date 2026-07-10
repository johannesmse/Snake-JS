https://johannes.oleherman.com

## Run offline / locally

The entire tool is self contained inside `index.html` - you can download this file and run it in your browser.

When this is deployed, it is running in a minimal nginx Dockerfile (just 2 lines).
You can run this locally as well, with `docker`:

```bash
docker build --tag johannes . && docker run -it -p 8000:80 --name johannes --rm johannes
```

Or with `podman`:

```bash
podman build --tag johannes . && podman run -it -p 8000:80 --name johannes --rm johannes
```

Open in the browser:

http://127.0.0.1:8000
