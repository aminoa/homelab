# Updating Cloudflare Config
    
kubectl create secret generic config-cloudflare-ddns -n cloudflare-ddns --from-file=config.json=config.json --dry-run=client -o yaml | kubeseal --format yaml > sealed-secret.yaml

