# 🧩 Swagger YAML Viewer

Um simples servidor em **Node.js + Express** para rodar arquivos **YAML** e visualizar sua documentação **Swagger UI** no navegador.

## 🚀 Tecnologias

* [Node.js](https://nodejs.org/)
* [Express](https://expressjs.com/)
* [Swagger UI Express](https://www.npmjs.com/package/swagger-ui-express)
* [YAMLJS](https://www.npmjs.com/package/yamljs)

## 📦 Instalação

Clone o repositório:

```bash
git clone https://github.com/seu-usuario/swagger-yaml-viewer.git
cd swagger-yaml-viewer
```

Instale as dependências:

```bash
npm install
```

## ▶️ Uso

1. Coloque seu arquivo `.yaml` (exemplo: `voting-system.yaml`) dentro da raiz do projeto.
2. No arquivo `index.js`, altere o caminho do YAML se necessário:

```js
const swaggerDocument = YAML.load(path.join(__dirname, 'SEU_ARQUIVO.yaml'));
```

3. Inicie o servidor:

```bash
node server.js
```

4. Acesse no navegador:

```
http://localhost:2000/api-docs
```

✨ Agora você terá sua documentação Swagger rodando localmente.

## 📁 Estrutura do projeto

```
swagger-yaml-viewer/
│── util               # Todos os teus arquivos YAML
│── index.js           # Código principal
│── package.json       # Dependências
│── voting-system.yaml # Exemplo de arquivo YAML
└── README.md
```

## 🛠 Scripts úteis

Adicionar no `package.json`:

```json
"scripts": {
  "start": "node index.js",
  "dev": "nodemon index.js"
}
```

Assim você pode rodar com:

```bash
npm run start
# ou em modo dev (auto reload):
npm run dev
```

## 🤝 Contribuições

Sinta-se livre para abrir **issues** e enviar **pull requests**.

## 📜 Licença

Distribuído sob a licença MIT. Veja `LICENSE` para mais informações.
