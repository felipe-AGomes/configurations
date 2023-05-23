### Teste em react (Vite) com Testing Library e Typescript

```bash
npm install jest ts-jest @types/jest @testing-library/jest-dom @testing-library/react @testing-library/user-event -D
```

##### Para não ter problemas quando os componentes que forem testados precisarem importar um arquivo de estilo

```bash
npm install identity-obj-proxy -D
```

Configuração do arquivo jest.config

```javascript

/* eslint-disable no-undef */
/** @type {import('ts-jest').JestConfigWithTsJest} */
module.exports = {
	preset: 'ts-jest',
	testEnvironment: 'jsdom',

	// Para importação dos estilos
	moduleNameMapper: {
		'\\.(css|less|sass|scss)$': 'identity-obj-proxy',
	},
};

```


### Teste em Node com Typescript

```bash
npm install jest @types/jest ts-jest -D
```

Configuração do arquivo jest.config

```javascript
/* eslint-disable no-undef */
/** @type {import('ts-jest').JestConfigWithTsJest} */
module.exports = {
	preset: 'jest',
	testEnvironment: 'node',
};
```
