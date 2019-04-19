# ![](https://avatars1.githubusercontent.com/u/8237355?v=2&s=50) Grav

[![PHPStan](https://img.shields.io/badge/PHPStan-enabled-brightgreen.svg?style=flat)](https://github.com/phpstan/phpstan)
[![SensioLabsInsight](https://insight.sensiolabs.com/projects/cfd20465-d0f8-4a0a-8444-467f5b5f16ad/mini.png)](https://insight.sensiolabs.com/projects/cfd20465-d0f8-4a0a-8444-467f5b5f16ad)
[![Discord](https://img.shields.io/discord/501836936584101899.svg?logo=discord&colorB=728ADA&label=Discord%20Chat)](https://chat.getgrav.org)
 [![Build Status](https://travis-ci.org/getgrav/grav.svg?branch=develop)](https://travis-ci.org/getgrav/grav) [![OpenCollective](https://opencollective.com/grav/backers/badge.svg)](#backers) [![OpenCollective](https://opencollective.com/grav/sponsors/badge.svg)](#sponsors)

O Grav é uma plataforma Web baseada em arquivos **rápida**, **simples**, e **flexível**. A necessidade de instalação é **ZERO**. Basta extrair o arquivo ZIP e já está instalado e funcionando. Ele segue princípios semelhantes a outras plataformas CMS de arquivos simples, mas tem uma filosofia de design diferente da maioria. Grav vem com um poderoso **sistema de gerenciamento de pacotes** para permitir a instalação e atualização simples de plugins e temas, bem como a simples atualização do próprio Grav.

A arquitetura subjacente do Grav foi projetada para usar tecnologias bem estabelecidas e de _primeira classe_ para garantir que o Grav seja simples de usar e fácil de estender. Algumas dessas tecnologias-chave incluem:

* [Twig Templating](https://twig.sensiolabs.org/): para um controle poderoso da interface do usuário
* [Markdown](https://en.wikipedia.org/wiki/Markdown): para facilitar a criação de conteúdo
* [YAML](https://yaml.org): para configuração simples
* [Parsedown](https://parsedown.org/): para suporte rápido a Markdown e Markdown Extra
* [Doctrine Cache](https://www.doctrine-project.org/projects/doctrine-orm/en/latest/reference/caching.html): camada para desempenho
* [Pimple Dependency Injection Container](https://pimple.sensiolabs.org/): para extensibilidade e manutenção
* [Symfony Event Dispatcher](https://symfony.com/doc/current/components/event_dispatcher/introduction.html): para manipulação de eventos de plug-in
* [Symfony Console](https://symfony.com/doc/current/components/console/introduction.html): para interface CLI
* [Gregwar Image Library](https://github.com/Gregwar/Image): para manipulação dinâmica de imagens

# Requisitos:

- PHP 7.1.3 ou superior. Verifique a [lista de móduloes necessários](https://learn.getgrav.org/basics/requirements#php-requirements)
- Verifique os requisitos do [Apache](https://learn.getgrav.org/basics/requirements#apache-requirements) ou do [IIS](https://learn.getgrav.org/basics/requirements#iis-requirements)

# Início rápido:

Estas são as opções para obter o Grav:

### Download de um pacote GRAV

Você pode baixar um pacote **pronto** na [Página de Downloads em https://getgrav.org](https://getgrav.org/downloads)

### Usando o Composer

Você pode criar um novo projeto com a última **versão estável** do Grav com o seguinte comando:

```
$ composer create-project getgrav/grav ~/webroot/grav
```

### Diretamente do GitHub

1. Clone o repositório do Grav em [https://github.com/getgrav/grav]() para uma pasta na webroot do seu servidor, por exemplo: `~/webroot/grav`. Inicie um **terminal** ou **console** e navegue até a pasta webroot:
   ```
   $ cd ~/webroot
   $ git clone https://github.com/getgrav/grav.git
   ```

2. Instale os **plugin's** e **dependências do tema** utilizando o [Grav CLI application](https://learn.getgrav.org/advanced/grav-cli) `bin/grav`:
   ```
   $ cd ~/webroot/grav
   $ bin/grav install
   ```

Confira os [procedimentos de instalação](https://learn.getgrav.org/basics/installation) para mais informações.

# Adicionando Funcionalidades

Você pode baixar [Plugins](https://getgrav.org/downloads/plugins) ou [Temas](https://getgrav.org/downloads/themes) manualmente a partir da guia apropriada na [Página de Downloads em https://getgrav.org](https://getgrav.org/downloads), mas a solução preferida é usar o [Gerenciador de Pacotes do Grav](https://learn.getgrav.org/advanced/grav-gpm) ou `GPM`:

```
$ bin/gpm index
```

Isto irá mostrar todos os plugins disponíveis e você pode instalar um ou mais com:

```
$ bin/gpm install <plugin/theme>
```

# Atualizações

Para atualizar o Grav você deve usar o [Gerenciador de Pacote do Grav](https://learn.getgrav.org/advanced/grav-gpm) ou `GPM`:

```
$ bin/gpm selfupgrade
```

Para atualizar plugins e temas:

```
$ bin/gpm update
```


# Contribuindo
We appreciate any contribution to Grav, whether it is related to bugs, grammar, or simply a suggestion or improvement! Please refer to the [Contributing guide](CONTRIBUTING.md) for more guidance on this topic.

## Security issues
If you discover a possible security issue related to Grav or one of its plugins, please email the core team at contact@getgrav.org and we'll address it as soon as possible.

# Getting Started

* [What is Grav?](https://learn.getgrav.org/basics/what-is-grav)
* [Install](https://learn.getgrav.org/basics/installation) Grav in few seconds
* Understand the [Configuration](https://learn.getgrav.org/basics/grav-configuration)
* Take a peek at our available free [Skeletons](https://getgrav.org/downloads/skeletons)
* If you have questions, jump on our [Discord Chat Server](https://chat.getgrav.org)!
* Have fun!

# Exploring More

* Have a look at our [Basic Tutorial](https://learn.getgrav.org/basics/basic-tutorial)
* Dive into more [advanced](https://learn.getgrav.org/advanced) functions
* Learn about the [Grav CLI](https://learn.getgrav.org/cli-console/grav-cli)
* Review examples in the [Grav Cookbook](https://learn.getgrav.org/cookbook)
* More [Awesome Grav Stuff](https://github.com/getgrav/awesome-grav)

# Backers
Support Grav with a monthly donation to help us continue development. [[Become a backer](https://opencollective.com/grav#backer)]

<img src="https://opencollective.com/grav/tiers/backers.svg?avatarHeight=36&width=600" />

# Sponsors
Become a sponsor and get your logo on our README on Github with a link to your site. [[Become a sponsor](https://opencollective.com/grav#sponsor)]

<img src="https://opencollective.com/grav/tiers/sponsors.svg?avatarHeight=36&width=600" />

# License

See [LICENSE](LICENSE.txt)


[gitflow-model]: http://nvie.com/posts/a-successful-git-branching-model/
[gitflow-extensions]: https://github.com/nvie/gitflow

# Running Tests

First install the dev dependencies by running `composer update` from the Grav root.
Then `composer test` will run the Unit Tests, which should be always executed successfully on any site.
Windows users should use the `composer test-windows` command.
You can also run a single unit test file, e.g. `composer test tests/unit/Grav/Common/AssetsTest.php`
