## Exemplo estrutura Babel JS 

_[Read in english](https://github.com/lynconEBB/babelJS-example/blob/master/README-en.md)_

Este repositório tem o objetivo de proporcionar um ambiente de desenvolvimento JavaScript capaz de utilizar as últimas funcionalidades ainda sendo compatível com os navegadores mais antigos

### Pré-requisitos

- Node
- NPM
- Git

### Instalação

Primeiramente clone este repositório no local em que achar mais adechado utilizando o seguindo comando:

```bash
git clone https://github.com/lynconEBB/babelJS-example.git
``` 

Após isso instale as dependências utilizadas com o seguinte comando:

```bash
npm install --dev
```

### Usando

Essa estrutura foi feita para ser o mais simples possível de usar, basta colocar seus codigos na pasta [src](https://github.com/lynconEBB/babelJS-example/tree/master/src) e o codigo convertido será colocado na pasta [out](https://github.com/lynconEBB/babelJS-example/tree/master/out).
 
Caso queira transformar os seus códigos apenas uma vez utilize o comando:

```bash
npm run build 
```

Ou caso queira escrever os seus códigos e automaticamente converte-los toda a vez que salvar, utilize o comando:
```bash
npm run watch
```

### Configuração

Todas as alterações nas configurações do Babel podem ser feitas no arquivo [babel.config.json](https://github.com/lynconEBB/babelJS-example/blob/master/babel.config.json).

Para alterar os navegadores que quer garantir compatibilidade basta alterar o parâmetro _targets_. Este parâmetro pode ser um objeto JSON contendo o nome dos navegadores e suas versões ou uma query no [formato browserslist](https://github.com/browserslist/browserslist#queries).

```JSON
{
"presets": 
[
  [
    "@babel/env",{
      "targets": {
        "chrome": "58",
        "ie": "11"  
      }  
    }
  ]
 ]
}
```