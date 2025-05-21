# Projeto: Servidor Web com Docker + Nginx

## 📌 Objetivo do Projeto

Este projeto tem como objetivo demonstrar como utilizar o **Docker** para criar uma imagem personalizada do **Nginx** que serve arquivos HTML e imagens estáticas. É uma aplicação simples para fins de estudo sobre **containers** e **servidores web**.

---

## 📁 Estrutura de Pastas

```
AVALIACAO-PAGLIACCI/
├── html/
│   ├── index.html
│   └── docke.webp
└── Dockerfile
```

---

## 🛠️ Comandos Utilizados

### ✅ Build da imagem personalizada

```bash
docker build -t nginx-app .
```

### ✅ Executar o container

```bash
docker run --name meu-site -p 8080:80 -d nginx-app
```

### ✅ Verificar containers em execução

```bash
docker ps
```

### ✅ Parar o container

```bash
docker stop meu-site
```

### ✅ Remover o container

```bash
docker rm meu-site
```

---

## 🚀 Como Executar o Projeto

1. Certifique-se de que o **Docker Desktop** está instalado e em execução no seu sistema.

2. Navegue até o diretório do projeto:

```bash
cd caminho/para/AVALIACAO-PAGLIACCI
```

3. Construa a imagem Docker com:

```bash
docker build -t nginx-app .
```

4. Execute o container mapeando a porta 8080:

```bash
docker run --name meu-site -p 8080:80 -d nginx-app
```

5. Acesse a aplicação no navegador:

```
http://localhost:8080
```

Você verá a página HTML personalizada sendo servida via Nginx.

---

## 👨‍💻 Autor

Projeto desenvolvido por **Pagliacci** como parte da avaliação de fundamentos de containers (Docker).
