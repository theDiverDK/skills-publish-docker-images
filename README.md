# Publish Docker Images

A GitHub Skills exercise for building a small static site into a Docker image and publishing it through GitHub Actions.

## What is in this repository

- `src/` — static HTML, JavaScript, CSS, and pattern assets served by Nginx.
- `Dockerfile` — packages `src/` into the `nginx:alpine` image.
- `.github/workflows/` — the guided exercise workflows.
- `.github/steps/` — instructions for each exercise step.

## Run locally

Build and start the container:

```bash
docker build -t publish-docker-images .
docker run --rm -p 8080:80 publish-docker-images
```

Then open <http://localhost:8080>.

## Exercise

Follow the tasks in [the exercise issue](https://github.com/theDiverDK/skills-publish-docker-images/issues/1). The workflow files advance the exercise through building and publishing a Docker image.

## License

See [LICENSE](LICENSE).
