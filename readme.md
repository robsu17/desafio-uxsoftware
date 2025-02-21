# Desafio UxSoftware  

Este projeto é um **proxy reverso** desenvolvido como parte do desafio da **UxSoftware**. Ele utiliza **Docker** para facilitar a configuração, implantação e gerenciamento dos serviços, garantindo **escalabilidade**, **isolamento** e **melhor controle do tráfego** entre clientes e servidores.  

## 🛠 Requisitos  

Antes de começar, certifique-se de ter as seguintes ferramentas instaladas:  

| Ferramenta | Descrição |
|------------|-----------|
| [Docker](https://www.docker.com/) | Plataforma para criar, implantar e executar containers. |
| [Docker Compose](https://docs.docker.com/compose/) | Orquestração de múltiplos containers. |

Você pode verificar se o Docker está instalado rodando:  
```sh
docker --version
```  
E para o Docker Compose:  
```sh
docker compose version
```

---

## 🚀 Como executar o projeto  

### 1️⃣ Clone o repositório:  
```sh
git clone https://github.com/robsu17/desafio-uxsoftware.git
```

### 2️⃣ Acesse o diretório do projeto:  
```sh
cd desafio-uxsoftware
```

### 3️⃣ Configure as variáveis de ambiente:  
Copie o arquivo de exemplo `.env.example` e renomeie para `.env`:  
```sh
cp .env.example .env
```

### 4️⃣ Execute o Docker Compose:  
Inicie os containers em segundo plano:  
```sh
docker compose up -d
```

O projeto estará rodando em: **[http://localhost:8080](http://localhost:8080)** 🚀  

---

## 💛 Como parar o projeto  
Para interromper os containers, utilize:  
```sh
docker compose down
```

---

## 📌 Exemplo de requisição  
Se o proxy reverso estiver configurado corretamente, você pode fazer uma requisição via `curl` para testá-lo:  
```sh
curl -i http://localhost:8080
```

Caso esteja funcionando, você verá a resposta do servidor configurado.  

---

