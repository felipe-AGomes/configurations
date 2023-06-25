### Configurações para utilizar express com typescript

#### Baixar dependencias

```bash
npm install express
npm install typescript ts-node-dev @types/express -D
```

#### Iniciar o typescript

```bash
npx tsc --init
```

#### Alterar em "scripts" no package.json

```json
"scripts": {
    "dev": "ts-node-dev src/server.ts"
}
```
