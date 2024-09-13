# Kryotogarten

## Dockerizaçao do site 

Construçao da aplicaçao e criacao da imagem que será publicada no docker hub. 

A aplicaçao executará na porta 4000, conforme o parâmetro -p do comando docker run. 


- Faça o build da imagem e a publica no `docker hub`:

```bash
docker build . -t juliozohar/kryptogarten:1.0

docker push juliozohar/kryptogarten:1.0
```

- Execute o container 

```bash
docker run -d -p 4000:3000 juliozohar/kryptogarten:1.0
```

- Acesse a aplicacao via browser pelo endereço : http://localhost:4000

Para acessar a estrutura do container docker

```bash
docker exec -it juliozohar/kryptogarten:1.0 /bin/sh
```