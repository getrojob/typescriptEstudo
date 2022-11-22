# typescriptEstudo

```bash
npm init -y
npm i typescript -D
```
Instalando o ts-node e Code Runner
```bash
npm i ts-node -D
```
Instalar run via extension

Criar dir .vscode para aplicar uma configuração personalizada
- Add settings.json
- Add dentro no settings
```javascript
"code-runner.executorMap": {
	"typescript": "npx ts-node --files"
	}
```
	
Aplicar o eslint
```bash
npm i eslint -D
```
Aplicar o plugin eslint e parser
```bash
npm i @typescript-eslint/eslint-plugin @typescript-eslint/parser -D
```
Add .eslintrc.js
	e o seguinte conteudo

```javascript
module.exports = {
    env: {
        browser: true,
        es6: true,
        node: true,
    },
    extends: [
        'eslint:recommended',
        'plugin:@typescript-eslint/eslint-recommended',
        'plugin:@typescript-eslint/recommended',
    ],
    globals: {
        Atomics: 'readonly',
        SharedArrayBuffer: 'readonly',
    },
    parser: '@typescript-eslint/parser',
    parserOptions: {
        ecmaVersion: 11,
        sourceType: 'module',
    },
    plugins: ['@typescript-eslint'],
    rules: {},
};

```
Aplicar o prettier, config e plugin
```bash
npm i prettier eslint-config-prettier eslint-plugin-prettier -D
```

Add o .prettierrc.js
    e o seguinte conteudo

```javascript
module.exports = {
  semi: true,
  trailingComma: 'all',
  singleQuote: true,
  printWidth: 80,
  tabWidth: 2,
}
```
