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

Antes de começarmos a falar sobre esse comando, devemos entender os estados dos arquivos no git.

- <b>Untracked:</b> são arquivos que existem no repositorio local, mas o Git não está ciente deles. Isso geralmente acontece com novos arquivos que ainda não foram adicionados no controle de versão.
- <b>Unmodified:</b> são arquivos que existem no repositorio local e não foram editados ou modificados.
- <b>Modified:</b> são arquivos que foram modificados ou editados no seu repositorio local.
- <b>Stage:</b> são arquivos que foram adicionados ao índice e estão prontos para serem commitados.

<center>
![image](https://github.com/Nando2003/git-commands/assets/80061398/93d06e65-e24c-43ba-8065-7d0181d38b73)
</center>


<!-- ![image](https://github.com/Nando2003/git-commands/assets/80061398/af55a955-b727-411d-8450-20f2eefe7565) -->


