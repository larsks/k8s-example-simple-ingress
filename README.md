You will probably want to replace the hostnames in `base/ingress.yaml`. To do so, create an overlay that patches the ingress (and deploy from the overlay rather than from `base`). There is an example in `overlays/example`; if you `kubectl apply -k overlays/example`, it will create an Ingress for `www.example.com` instead of `example.apps.infra.house`.
