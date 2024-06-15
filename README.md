# Comandos Git para Iniciantes
Bem-vindo ao guia "Comandos Git para Iniciantes". Neste README.md, Você encontrá uma introdução aos conceitos básicos do Git, a ferramenta de controle de versão mais popular do mundo. Se você está começando sua jornada na área de desenvolvimento, este guia é feito para você. Aqui, você aprenderá como aplicar Git de maneira prática em seus futuros projetos, tornando seu fluxo de trabalho mais organizado e colaborativo.

## Quem sou eu?
Olá, meu nome é [Fernando Luiz Farias Fontes](https://github.com/Nando2003/Nando2003). Atualmente, estou cursando Ciência da Computação na Universidade Estácio de Sá e faço parte do laboratório [Fuzzlab-UVA](https://github.com/FuzzyLab-UVA), onde atuo como desenvolvedor back-end especializado em Django e REST Framework.

Desde cedo, sempre tive uma forte conexão com a tecnologia, mas foi após escrever meu primeiro "Hello World" que realmente me apaixonei por esta área tão incrível, que está presente no nosso dia a dia em todos os lugares. E estou aqui agora para passar um pouco do que eu sei sobre a ferramenta que é indispensável em qualquer projeto minimamente estruturado e organizado, que é o Git.

## Configuração Incial

```bash
$ git config --global user.name "Seu Username"
$ git config --global user.email "Email da sua conta no github"
```

O comando ```git config``` é usado para configurar variáveis de configuração do Git, e essas variáveis controlam o comportamento do Git em vários aspectos. As configurações ```user.name``` e ```user.email``` são utilizadas para identificar quem fez um commit dentro de um repositório, sendo informações importantes para atribuir autoria aos commits. Essas configurações são essenciais para garantir a integridade e a rastreabilidade do histórico de commits de um projeto Git.


## Iniciando um Repositório Local

```bash
$ git init
```

O ```git init``` é um dos comandos mais fundamentais e importantes no Git. Ele é utilizado para criar um novo repositório Git em um diretório existente ou para inicializar um repositório vazio para começar a usar o controle de versão. 

Quando o ```git init``` é executado em um diretório, o Git cria um subdiretório oculto chamado .git, que contém todos os arquivos necessários para o repositório. Esses arquivos incluem o histórico de revisões, as configurações do repositório e outros metadados que o Git usa para rastrear as alterações no projeto.

![image](https://github.com/Nando2003/git-commands/assets/80061398/b4eb4540-ba97-49ed-b89e-9cc60be068c4)

## Verificação do Status

```bash
$ git status
```

O comando ```git status``` é utilizado para mostrar o estado de cada arquivo e pasta dentro do seu repositorio local. Os estados que você pode encontrar eles, são:

- <b>Untracked:</b> são arquivos que existem no repositorio local, mas o Git não está ciente deles. Isso geralmente acontece com novos arquivos que ainda não foram adicionados no controle de versão.
- <b>Unmodified:</b> são arquivos que existem no repositorio local e não foram editados ou modificados.
- <b>Modified:</b> são arquivos que foram modificados ou editados no seu repositorio local.
- <b>Stage:</b> são arquivos que foram adicionados ao índice e estão prontos para serem commitados.

![image](images/lifecycle.png)

> Imagem retidada do site [Oficial do Git](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository)

## Adição de arquivos e pastas ao índice

```bash
$ git add <arquivo>
$ git add .
```

O comando ```git add``` é utilizado para adicionar arquivos ao índice, preparando-os para serem incluídos no próximo commit. Ele não apenas adiciona arquivos modificados, mas também arquivos untracked ao estado Staged.

## Commitando as Alterações

```bash
$ git commit -m "Descreva a alteração"
```

Chegamos no sujeito mais balado do git, o ```git commit```. Esse comando é responsavel por levar as mudanças de um ambiente local para o repositório no git, permitindo a adição de uma mensagem que descreva o que foi alterado. Essa parte é de grande importancia para os 
desenvolvedores, pois permite que eles documentem as alterações feitas no código, facilitando o entendimento do histórico de desenvolvimento do projeto e ajudando na colaboração em equipe.

### Como escrever um commit?

Para aprendermos a escrever commits, precisamos primeiramente entender a padronização.

Um projeto com commits bem organizados é um projeto que <b>documenta um histórico</b>. Ele mostra o que foi feito ao longo do tempo, criando um registro detalhado. Então é necessário que tenha uma padronização como as coisas são entregues para que o código não fique uma bagunça e que <b>todos se entendam</b>. 

#### Algumas tipos de commits:

- (feat): Incluir um novo recurso.
- (wip): Indica que você ainda não terminou o que estava fazendo.
- (fix): Uma correção de bug foi realizada.
- (refractor): melhorias no código sem alterar a funcionalidade, como na legibilidade.
- (test): você criou ou corrigiu um teste.
- (docs): alteração na documentação, por exemplo: eu adicionei mais informação a esse README.md, então meu commit seria:

```bash
$ git commit -m "(doc) explicação mais detalhada sobre git commit foi adicionada"
```

## Entendendo como as Branches

As Branches são ramificações no Git que permitem que os desenvolvedores desenvolvam recursos, corrija erros ou experimente com segurança novas ideias em uma área sepada do seu repositório.

Uma Branch é criada a partir de uma existe. Por exemplo, quando temos é branch-padrão, casualmente chamada de main ou master, e precisamos desenvolver o back-end separadamente do front-end então nos criamos branchs diferentes a partir de um ponto de começo e depois unidas a partir de merge na branch-padrão.

![Diagrama sem nome drawio (8)](https://github.com/Nando2003/git-commands/assets/80061398/2f10779c-aab2-4768-b94d-4b7e7b1f1c6b)







