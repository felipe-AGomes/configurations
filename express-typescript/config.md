### Configurações para utilizar express com typescript

#### Baixar dependencias

```bash
npm install express
npm install typescript ts-node @types/express -D
```

#### Iniciar o typescript

```bash
npx tsc --init
```

#### Alterar em "scripts" no package.json

```json
"scripts": {
    "dev": "ts-node src/server.ts"
}
```
