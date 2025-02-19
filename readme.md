## Desafio Uxsoftware 
Este projeto é um proxy reverso desenvolvido como parte do desafio da UxSoftware. Ele utiliza Docker para facilitar a configuração, implantação e gerenciamento dos serviços, garantindo escalabilidade, isolamento e melhor controle do tráfego entre clientes e servidores.

## Requisitos do projeto  

| Ferramenta | Ícone |
|------------|-------|
| [Docker](https://www.docker.com/) | ![Docker](https://img.icons8.com/?size=32&id=cdYUlRaag9G9&format=png&color=000000) |

## Como executar o projeto

### 1. Clone o respositório:

```
git clone https://github.com/robsu17/desafio-uxsoftware.git
```

### 2. Configure as variáveis de ambiente

```
cp .env.example .env
```
### 3. Execute o Docker compose:
```
  docker compose up -d
```