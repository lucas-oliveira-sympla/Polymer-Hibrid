![Polymer Hibrid](https://www.polymer-project.org/images/logos/p-logo.png)
# Polymer-Hibrid
---
Caso você possua uma aplicação rodando Polymer 1 e queria migrar para Polymer 2 existe uma solução, trabalhar com uma aplicação hibrida onde você podera continuar usando seus elementos Polymer 1 e escrever os novos componentes com Polymer 2.

Projeto com polymer 1

link aqui

Projeto com suporte a Polymer 1 e 2

link aqui


## Detalhes
---

Temos que alterar o nossos modo de gerencias as dependencias no Bower:

```
    {
        "name": "my-application",
        "authors": [
            "your name <youremail@gmail.com>"
        ],
        "description": "",
        "main": "",
        "license": "MIT",
        "ignore": [
            "**/.*",
            "node_modules",
            "bower_components",
            "bower_components-1.x",
            "test",
            "tests"
        ],
        "dependencies": {
            "polymer": "Polymer/polymer#1.11.3 - 2",
            "paper-button": "PolymerElements/paper-button#2.1.3",
            "webcomponentsjs": "webcomponents/webcomponentsjs#^1.0.0"
        },
        "variants": {
            "1.x": {
                "dependencies": {
                    "polymer": "Polymer/polymer#1.11.3",
                    "webcomponentsjs": "webcomponents/webcomponentsjs#^0.7.0"
                },
                "resolutions": {
                    "webcomponentsjs": "^0.7"
                }
            }
        },
        "resolutions": {
            "webcomponentsjs": "^1.0.0"
        }
    }
```







