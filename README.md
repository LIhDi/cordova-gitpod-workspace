<br />
<p align="center">
  <a href="https://www.gitpod.io/">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3f/Gitpod-ddd.svg/512px-Gitpod-ddd.svg.png" alt="Logo">
  </a>
</p>

## Conteúdo

- [Sobre o Projeto](#sobre-o-projeto)
- [Começando](#come%C3%A7ando)
  - [Instalação](#instala%C3%A7%C3%A3o)
  - [Novo Projeto](#novo-projeto)
  - [Desenvolvimento](#desenvolvimento)
- [Contribuição](#contribui%C3%A7%C3%A3o)
- [Licença](#licen%C3%A7a)


## Sobre o Projeto

Cordova Gitpod Workspace - é um projeto onde temos algumas configurações para ser possível ter um ambiente online de desenvolvimento de aplicações híbridas.
Este projeto surgiu da necessidade dos alunos da turma de **Desenvolvimento de Aplicações Móveis** ao qual frequento, não conseguirem desenvolver em sala de aula os projetos propostos pelo professor.

## Começando

### Instalação

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io#snapshot/92522914-a004-4212-900f-896e2aec1577)


- Fazer o login e autorizar o Gitpod no Github.
- Assim que abrir o container aceitar todas as permissões [y] ou [A]
- Entrar no contexto do ambiente

```sh
cd /workspace/cordova-gitpod-workspace
```

### Novo Projeto

```sh
cordova create new-app
cd new-app/
cordova platform add android
cordova run android
```
### Desenvolvimento

Para rodar o projeto:

Ainda vai ser configurado essa parte, será pensado a melhor estratégia

Para dar o build no projeto e gerar o apk:

```sh
cordova build android --no-telemetry
```
O apk gerado estará no path platforms/android/app/build/outputs/apk/debug/
Poderá baixar e rodar no telefone


## Contribuição

1. Faça o _fork_ do projeto (`https://github.com/LihDi/cordova-gitpod-worksapce/fork`)
2. Crie um _branch_ para sua modificação (`git checkout -b feature/fooBar`)
3. Adicione suas mudanças (`git add .`)
4. Faça o _commit_ (`git commit -am 'Add some fooBar'`)
5. Faça o _Push_ (`git push origin feature/fooBar`)
6. Crie um novo _Pull Request_

## Licença

Distribuído sob a licença MIT. Veja `LICENSE` para mais informações.
