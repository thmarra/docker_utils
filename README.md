# Docker + Docker compose

**OBS:** 
- Os volumes do mongo e postgres precisam estar apontando pra um disco que não esteja formatado como NTFS. Pelo menos até então não consegui inicar os containers quando os volumes estão apontando pra uma partição NTFS #helpwanted

**Iniciando um container:**
- Precisa ter tanto o Docker quanto o Docker compose instalados

`docker-compose -f docker-compose.service.yml up -d --build`
- `-f, --file FILE`:  informa qual arquivo deve ser utilizado para iniciar o serviço (default: docker-compose.yml)
- `-d, --detach`:  Detached mode - executa o container em background
- `--build`: Monta a imagem antes de iniciar o container

**Documentação:**

[Docker](https://docs.docker.com/engine/reference/run/)

[Docker compose](https://docs.docker.com/compose/reference/overview/)