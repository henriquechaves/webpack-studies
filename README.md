# webpack-studies

O Webpack é o principal pacote de módulos para aplicativos React e Redux. 

# Webpack’s Core Philosophy

As principais filosofias do webpack são?

1) Tudo é um módulo  - Isso significa que podemos dividir qualquer artefato em peças menores gerenciáveis, reutilizá-los e assim sucessivamente.

2) Carregue apenas o que precisa e enquanto precisa - permite dividir seu código e gerar vários arquivos de <strong>bundle</strong>, e também carregar partes do aplicativo de forma assíncrona para que você manipule o que pretenda usar

# Development Vs Production

Seu código pode ser estruturado de modo que possa trabalhar “Development-only”, “Production-only” e“Production-and-Development”.

Scripts no package.json

```js
"Scripts": { 
  // npm run build para construir bundles de produção 
  "build": "webpack --config webpack.config.prod.js",
  // npm run dev para gerar bundles de desenvolvimento e executar dev. Servidor 
  "dev": "webpack-dev-server" 
}
```

# webpack CLI Vs webpack-dev-server

Nota-se que em webpack o módulo bundler fornece duas interfaces:

- Webpack CLI tool  —  the default interface (Instalada pelo próprio Webpack)