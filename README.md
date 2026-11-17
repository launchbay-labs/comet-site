# comet-site



Launched with [Launchbay](https://github.com/paighanutkarsh2410-lab/launchbay) from the **Static Site** template.

## Run locally

```bash
docker build -t comet-site . && docker run -p 8080:8080 comet-site
```

## Delivery

Every push to `main` is tested, scanned with Trivy, built, pushed to GHCR and signed with cosign.
Launchbay's GitOps repo points Argo CD at the image, and the service is served at
`http://comet-site.localtest.me`.
