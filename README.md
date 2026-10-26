# n8n-enterprise

Auto patch n8n stable builds

---

## ⚠️ Important Usage Notice: Non-Commercial & Research Only

**This project and all associated code, data, models, and documentation are provided strictly for research, educational, and academic purposes.**

- **DO NOT SELL:** This repository, its contents, or any derivative works created from it may **NOT** be sold, rented, licensed, or otherwise commercialized under any circumstances.
- **NON-COMMERCIAL USE ONLY:** Any commercial use, including using this work in a product or service offered for profit, is strictly prohibited.

## Get started

Just follow the official guide but replace the image name and tag.

```bash
docker volume create n8n_data

docker run -it --rm \
 --name n8n \
 -p 5678:5678 \
 -e GENERIC_TIMEZONE="<YOUR_TIMEZONE>" \
 -e TZ="<YOUR_TIMEZONE>" \
 -e N8N_ENFORCE_SETTINGS_FILE_PERMISSIONS=true \
 -v n8n_data:/home/node/.n8n \
 ghcr.io/appgifts/n8n-enterprise/n8n:latest
```
