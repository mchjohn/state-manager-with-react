# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
   parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
   },
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list


# Padrões usado
## Observable

O padrão Observable é um padrão de design de software que é usado para implementar a comunicação entre objetos. Ele permite que um objeto, chamado de "observável" ou "sujeito", notifique outros objetos, chamados de "observadores", sobre mudanças em seu estado.

Basicamente, o padrão Observable funciona da seguinte forma: um objeto observável mantém uma lista de seus observadores e fornece métodos para adicionar, remover e notificar esses observadores. Quando ocorre uma mudança no estado do objeto observável, ele notifica todos os observadores registrados, geralmente chamando um método específico em cada observador.
