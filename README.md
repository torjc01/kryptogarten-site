# Kryotogarten

## Dockerizaçao do site 

Faça o build da imagem 

```bash
docker build . -t kryptogarten
```

Execute o container 

```bash
docker run -p 4000:4000 kryptogarten
```

Acesse a aplicacao via browser pelo endereço : http://localhost:4000

Para acessar a estrutura do container docker: 

```bash
docker exec -it kryptogarten /bin/sh
```