# Typescript
Como criar um projeto typescript

Para criar um projeto com TypeScript, você pode seguir esses passos básicos. Vou guiar você pelo processo:

1. Pré-requisitos

Node.js e npm: Verifique se estão instalados, pois você precisará deles para gerenciar pacotes e dependências.

node -v
npm -v


2. Crie uma pasta para o projeto

Crie uma nova pasta e navegue até ela:

mkdir meu-projeto-typescript
cd meu-projeto-typescript


3. Inicie o projeto npm

Inicialize o projeto com o comando npm init. Isso criará o arquivo package.json:

npm init -y


4. Instale o TypeScript

Instale o TypeScript como dependência de desenvolvimento:

npm install typescript --save-dev


5. Configure o TypeScript

Crie o arquivo de configuração tsconfig.json, que define as opções de compilação. Para isso, execute:

npx tsc --init

Isso gerará um arquivo tsconfig.json com várias opções. As mais comuns para configurar são:

"target": Define a versão do JavaScript de saída. Exemplo: "target": "es6".

"outDir": Onde os arquivos JavaScript serão gerados após a compilação. Exemplo: "outDir": "./dist".

"rootDir": Define o diretório onde os arquivos TypeScript estão localizados. Exemplo: "rootDir": "./src".



6. Crie a estrutura do projeto

Crie uma pasta src onde você colocará seus arquivos TypeScript:

mkdir src

Dentro de src, crie seu primeiro arquivo TypeScript. Exemplo: src/index.ts.


7. Escreva código TypeScript

No arquivo src/index.ts, escreva um código simples:

const mensagem: string = "Hello, TypeScript!";
console.log(mensagem);


8. Compile o TypeScript para JavaScript

Para compilar o projeto, execute:

npx tsc

Isso criará um arquivo index.js na pasta dist, que é o código JavaScript gerado.


9. Execute o código JavaScript

Execute o código usando Node.js:

node dist/index.js


10. Automatize com npm scripts

No package.json, adicione scripts para facilitar o processo de compilação e execução:

"scripts": {
  "build": "tsc",
  "start": "node dist/index.js"
}


Agora você pode compilar e executar o projeto apenas com:

npm run build
npm start

Dicas adicionais

Instalar typings: Se usar bibliotecas JavaScript, você pode instalar tipos com @types para melhorar a integração com TypeScript. Exemplo: npm install @types/express --save-dev para o Express.


Assim, você já terá um projeto TypeScript básico configurado e pronto para desenvolvimento!


