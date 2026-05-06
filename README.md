# 📘 Miniguia de Estudos: Git e GitHub

## Contexto e Objetivos

Este projeto foi desenvolvido com o objetivo de utilizar Inteligência Artificial como ferramenta de apoio ao aprendizado sobre Git e Github, organizando e sintetizando conteúdos do tema com o uso do [NotebookLM](https://notebooklm.google.com/). Além disso, sua elaboração faz parte do atendimento ao desafio proposto no curso [Afya - Data Automation With AI](https://www.dio.me/en/bootcamp/afya-dados-bootcamp).

Tema escolhido: **Git e GitHub para iniciantes**

Objetivos:
- Entender os conceitos principais do tema
- Aprender os principais comandos e funções
- Utilizar a IA para estudos de conteúdos técnicos

---

## Fontes

As seguintes fontes foram utilizadas no NotebookLM:

1. https://git-scm.com/docs/git
2. https://docs.github.com/
3. https://www.freecodecamp.org/news/git-and-github-for-beginners/
4. https://www.atlassian.com/git/tutorials
5. https://www.youtube.com/watch?v=mAFoROnOfHs

---

## Testes de Prompts

### 🔹 Prompt 1
**Pergunta:**
> Defina o que são Git e GitHub para um iniciante.

**Resumo da resposta:**

Embora sejam termos frequentemente usados juntos, Git e GitHub não são a mesma coisa. Eles estão conectados, mas possuem funções distintas: o Git é o café e o GitHub é a cafeteria onde esse café é servido. O Git é um Sistema de Controle de Versões (VCS) de código aberto que funciona localmente no seu computador e tem como principal objetivo permitir que diferentes versões de um projeto sejam salvas. O GitHub é uma plataforma baseada na nuvem que hospeda repositórios Git. Em resumo, você usa o Git para organizar e salvar o progresso do seu trabalho localmente e o GitHub para armazenar esse trabalho na nuvem e colaborar com outras pessoas.

---

### 🔹 Prompt 2
**Pergunta:**
> Quais são as principais funcionalidades do Git e do GitHub?

**Resposta:**

As principais funcionalidades do Git e do GitHub dividem-se entre o controle de versões realizado localmente e as ferramentas de colaboração e hospedagem na nuvem.

*Principais Funcionalidades do Git (Local):*
- Rastreamento de Alterações: O Git monitora cada mudança feita nos arquivos (quem mudou, o que mudou e quando), permitindo um registro completo do histórico do projeto.
- Controle de Versão e "Viagem no Tempo": Ele permite salvar diferentes estados do seu trabalho. Caso ocorra um erro, você pode reverter para qualquer versão anterior sem perder dados.
- Fluxo de Trabalho em Três Áreas: O Git organiza o trabalho em três estágios: o diretório de trabalho (onde você edita os arquivos), a área de palco (staging) (onde você prepara as mudanças) e o repositório local (onde as mudanças são salvas permanentemente por meio de um commit).
- Branching (Ramificações): Permite criar cópias independentes do projeto para desenvolver novas funcionalidades ou testar ideias sem afetar o código principal ("main").
- Merging (Fusão): Após testar alterações em um branch separado, o Git permite combinar essas mudanças de volta ao projeto principal.
- Stashing: Uma ferramenta para armazenar temporariamente trabalhos inacabados, permitindo que você mude de tarefa ou de branch sem perder o progresso atual ou ser forçado a fazer um commit prematuro.

*Principais Funcionalidades do GitHub (Nuvem):*
- Hospedagem Remota e Backup: Atua como um servidor central seguro onde você pode enviar seus repositórios locais, servindo como um backup na nuvem acessível de qualquer lugar.
- Colaboração em Equipe: Centraliza o trabalho de vários desenvolvedores, permitindo que todos enviem suas atualizações e mantenham o projeto sincronizado em um único lugar. 
- Pull Requests (Solicitações de Pull): É a funcionalidade central para colaboração, onde um desenvolvedor solicita que suas alterações sejam revisadas e integradas ao projeto principal por outros membros da equipe.
- Gerenciamento de Projetos: Oferece ferramentas integradas como Issues (para rastrear problemas e tarefas) e quadros de projetos.
- Comunidade e Open Source: Facilita a descoberta e contribuição em projetos de código aberto ao redor do mundo.

*Funcionalidades de Integração (comandos que conectam o Git ao GitHub):*
- Push (Enviar): Envia seus commits locais para o repositório remoto no GitHub.
- Fetch e Pull (Trazer): O fetch baixa as novidades do servidor para o seu computador, enquanto o pull baixa e já as integra automaticamente ao seu diretório de trabalho.
- Clone: Cria uma cópia local de um projeto que já existe no GitHub para que você possa começar a trabalhar nele.
---

### 🔹 Prompt 3
**Pergunta:**
> Crie um passo a passo para um iniciante aprender a utilizar Git e GitHub , explicando os conceitos associados à cada etapa

**Resposta:**

Este guia passo a passo foi elaborado para ajudar um iniciante a dominar o Git (o "café") e o GitHub (a "cafeteria").

*1. Instalação e Verificação*

O primeiro passo é instalar o Git, que é a ferramenta que rodará localmente no seu computador para rastrear alterações.

- Ação: Baixe o Git no site oficial para o seu sistema operacional (Windows, Mac ou Linux).
- Comando: No terminal (ou Git Bash), digite git --version para confirmar se a instalação foi bem-sucedida.
- Conceito: O Git funciona como um rastreador que registra quem mudou o quê e quando.

*2. Configuração Inicial de Identidade*

Antes de salvar qualquer trabalho, o Git precisa saber quem você é para atribuir as alterações ao autor correto.

- Ação: Configure seu nome e e-mail globalmente.
- Comandos: <br>
   git config --global user.name "Seu Nome" <br>
   git config --global user.email "seuemail@exemplo.com"

*3. Criação e Inicialização do Projeto*

Um projeto monitorado pelo Git é chamado de Repositório.

- Ação: Crie uma pasta para seu projeto e entre nela pelo terminal usando comandos como mkdir e cd.
- Comando: Digite git init dentro da pasta.
- Conceito: O comando git init cria uma pasta oculta .git onde o histórico e os dados internos do projeto serão armazenados.

*4. O Fluxo de Trabalho Básico (Add e Commit)*

O Git organiza as alterações em três estados principais: Diretório de Trabalho, Área de Palco (Staging) e Repositório Local.

- Modificar: Crie ou edite arquivos na sua pasta (Working Directory).
- Preparar: Use git add . (ou o nome do arquivo) para mover as mudanças para a Staging Area. Esta é uma zona intermediária para revisão.
- Salvar: Use git commit -m "mensagem descritiva" para salvar permanentemente no Repositório Local.
- Conceito: Um Commit é como uma "foto" ou instantâneo do estado atual do seu código; você pode voltar a essa versão a qualquer momento. Use git status com frequência para ver em que estágio seus arquivos estão.

*5. Configuração do GitHub (Repositório Remoto)*

O GitHub é onde você armazena seus projetos na nuvem para backup ou colaboração.

- Ação: Crie uma conta no GitHub e clique em "New Repository" para criar um espaço para seu projeto online.
- Conceito: O Repositório Remoto funciona como um Google Drive para programadores, mantendo seu código seguro fora da sua máquina.

*7. Conectando Local e Remoto (Push e Clone)*

Agora você precisa enviar seu trabalho local para a nuvem.

- Conectar: Use git remote add origin [URL_DO_GITHUB] para vincular sua pasta local ao repositório online.
- Enviar: Use git push -u origin main para fazer o upload dos seus commits.
- Clonar: Se quiser baixar um projeto existente do GitHub para outro computador, use git clone [URL].

*8. Branching e Colaboração*

Para trabalhar em novas funcionalidades sem estragar o código principal, usamos Branches (ramificações).

- Criar Branch: git checkout -b nome-da-branch cria uma "cozinha de testes" separada do projeto principal.
- Merge: Após testar e commitar na branch, você usa git merge para combinar essas mudanças de volta à ramificação principal (main).
- Pull Request (PR): No GitHub, um PR é uma solicitação formal para que outros revisem seu código antes de ele ser integrado ao projeto oficial.

*9. Sincronização de Alterações*

Se você ou um colega fizerem mudanças diretamente no GitHub, você precisará atualizar seu computador local.

- Comando: git pull busca as novidades da nuvem e as integra automaticamente ao seu código local.
- Conceito: O Pull garante que você sempre trabalhe na versão mais recente do projeto.

---

### Dificuldades encontradas

- Respostas um pouco genéricas e repetitivas, exigindo uma maior detalhamento no prompt
- Formato de saída diferente do esperado, podendo ser melhorado com a especificação do formato no prompt  

---

## 📖 Miniguia de Estudo

### 📌 Resumo

Git é um sistema de controle de versão distribuído que permite rastrear alterações em arquivos ao longo do tempo, facilitando o gerenciamento de versões e o desenvolvimento de projetos de forma organizada.

O GitHub complementa o uso do Git ao oferecer uma plataforma na nuvem para hospedagem de repositórios, possibilitando colaboração entre desenvolvedores, compartilhamento de código e backup dos projetos.

---

### 📚 Glossário

- **Repositório:** Local onde o projeto e seu histórico de versões são armazenados  
- **Commit:** Registro de uma alteração realizada no projeto  
- **Branch:** Linha de desenvolvimento independente utilizada para trabalhar em funcionalidades separadas  
- **Merge:** Processo de integração entre diferentes branches  
- **Clone:** Cópia local de um repositório remoto  
- **Push:** Envio de alterações do repositório local para o remoto  
- **Pull:** Atualização do repositório local com alterações do remoto  

---

### 🔁 Sugestão de Prompts 

- "Explique Git e GitHub de forma simples para iniciantes"
- "Qual a diferença entre Git e GitHub?"
- "Explique passo a passo como realizar um commit"
- "O que diferencia um iniciante de um intermediário no uso do Git e do GitHub?"

