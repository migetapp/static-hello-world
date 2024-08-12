# static-hello-world

A barebone static page app using [httpd](https://httpd.apache.org/).

## Running Locally with `pack` and `docker`

Make sure you have [Docker](https://www.docker.com/) and [pack CLI](https://github.com/buildpacks/pack) installed.

```sh
$ pack config default-builder paketobuildpacks/builder-jammy-full
$ pack build static-hello-world
$ docker run -p 5000:5000 -e PORT=5000 static-hello-world
```

Your app should now be running on [localhost:5000](http://localhost:5000/).
