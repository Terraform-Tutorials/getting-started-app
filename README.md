## Containeriza uma app
Ao longo desta aula, você trabalhará com um gerenciador simples de lista de tarefas que roda em Node.js. Se você não estiver familiarizado com Node.js, não se preocupe. Este guia não exige nenhuma experiência prévia com JavaScript.

## Pré-requisitos

- Você instalou a versão mais recente do Docker. 
- Você instalou um cliente Git. 
- Você possui um IDE ou um editor de texto para editar arquivos.

## App (Lista de Tarefas)

```bash
git clone https://github.com/docker/getting-started-app.git
```

1. Alguns recursos que temos dentro dessa app abaixo:

```bash
$ tree getting-started-app/
getting-started-app/
├── README.md
├── package.json
├── spec
│   ├── persistence
│   │   └── sqlite.spec.js
│   └── routes
│       ├── addItem.spec.js
│       ├── deleteItem.spec.js
│       ├── getItems.spec.js
│       └── updateItem.spec.js
├── src
│   ├── index.js
│   ├── persistence
│   │   ├── index.js
│   │   ├── mysql.js
│   │   └── sqlite.js
│   ├── routes
│   │   ├── addItem.js
│   │   ├── deleteItem.js
│   │   ├── getItems.js
│   │   └── updateItem.js
│   └── static
│       ├── css
│       │   ├── bootstrap.min.css
│       │   ├── font-awesome
│       │   │   ├── all.min.css
│       │   │   ├── fa-brands-400.eot
│       │   │   ├── fa-brands-400.svg#fontawesome
│       │   │   ├── fa-brands-400.ttf
│       │   │   ├── fa-brands-400.woff
│       │   │   ├── fa-brands-400.woff2
│       │   │   ├── fa-regular-400.eot
│       │   │   ├── fa-regular-400.svg#fontawesome
│       │   │   ├── fa-regular-400.ttf
│       │   │   ├── fa-regular-400.woff
│       │   │   ├── fa-regular-400.woff2
│       │   │   ├── fa-solid-900.eot
│       │   │   ├── fa-solid-900.svg#fontawesome
│       │   │   ├── fa-solid-900.ttf
│       │   │   ├── fa-solid-900.woff
│       │   │   └── fa-solid-900.woff2
│       │   └── styles.css
│       ├── index.html
│       └── js
│           ├── app.js
│           ├── babel.min.js
│           ├── react-bootstrap.js
│           ├── react-dom.production.min.js
│           └── react.production.min.js
└── yarn.lock

11 directories, 40 files
```

