Learning using tutorials from n8n.io
https://docs.n8n.io/hosting/installation/docker/#prerequisites

```
docker volume create n8n_data
docker run -it --rm --name n8n -p 5678:5678 -v n8n_data:/home/node/.n8n docker.n8n.io/n8nio/n8n
```


Starting with a timezone

```
docker run -it --rm \
 --name n8n \
 -p 5678:5678 \
 -e GENERIC_TIMEZONE="America/New_York" \
 -e TZ="America/New_York" \
 -v n8n_data:/home/node/.n8n \
 docker.n8n.io/n8nio/n8n
```


