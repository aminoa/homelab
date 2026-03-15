# Homelab

These are the Kubernetes configs that are running on my k3s home laptop cluster. I have written further on the [homelab wiki](https://homelab.aneeshmaganti.com). 

## Notes

- cloudflare-ddns: `config.json` controls which endpoints have their DNS updated; since the entire config.json is in a sealed secret, configuration changes require re-sealing the entire config. 
- romm is set to only 1 replica since the romm-library is set to ReadWriteOnce (which can provide better performance).