# QAQ 
```bash
clone this repo
cp ~/.docker/config.json qaq/config.json
openssl genrsa -out qaq/private_key.pem 1024
openssl rsa -in qaq/private_key.pem -pubout -out qaq/public_key.pem
# edit qaq/kustomization.yaml set the correct values
kubectl apply -k qaq
```