# 🎵 Playlist do projeto 2 de JS

Player de música feito com **HTML, CSS e JavaScript puro** (sem frameworks, sem build step), como projeto final do curso de JavaScript do Instituto 3C.

## Funcionalidades

- Play / pause
- Próxima / música anterior
- Barra de progresso clicável (seek)
- Modo aleatório (shuffle)
- Repetir música
- Curtir música (favoritos salvos no `localStorage`)

## Playlist

1. **Taça de Pranto** — Gian e Giovani
2. **Chega** — Zezé Di Camargo e Luciano
3. **Sublime Renúncia** — Leandro e Leonardo

## Tecnologias

- HTML5 semântico
- CSS3
- JavaScript (Vanilla)
- Docker + Docker Compose (Nginx)

## Como rodar com Docker

Pré-requisitos: [Docker](https://www.docker.com/) e Docker Compose instalados.

```bash
git clone https://github.com/matheuspidorodeski/projetojs2-3c.git
cd projetojs2-3c
docker compose up --build
```

Depois acesse: **http://localhost:8080**

Para parar o container:

```bash
docker compose down
```

## Como rodar sem Docker

Basta abrir o arquivo `index.html` diretamente no navegador, ou servir a pasta com qualquer servidor estático (ex: extensão Live Server do VS Code).

## Estrutura do projeto

```
projetojs2-3c/
├── images/         # Capas dos álbuns
├── songs/          # Arquivos de áudio (.mp3)
├── index.html
├── style.css
├── script.js
├── Dockerfile
└── docker-compose.yml
```

## Observações

Os arquivos de áudio podem nao estar incluídos no repositório por questao de bug. Para o player funcionar, adicione os arquivos `.mp3` correspondentes na pasta `songs/` com os nomes exatamente como referenciados no `script.js`.
