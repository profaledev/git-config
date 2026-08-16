Aqui está um guia completo e detalhado em formato Markdown (`.md`). Você pode copiar esse código e colar diretamente em um arquivo (por exemplo, `GUIA-GIT.md`) no seu repositório ou postar na plataforma que utiliza com seus alunos da Etec.

Ele foi pensado para ser lido de forma fácil por quem está começando, usando os repositórios reais da nossa disciplina como exemplo prático.

---

```markdown
# 🚀 Guia Definitivo: Git, GitHub e o Fluxo das Nossas Aulas

Olá, turma! Tudo bem?

Para que possamos organizar nossos projetos de Sistemas Web, HTML, CSS e JavaScript, vamos utilizar o **Git** e o **GitHub**. Este guia vai ensinar desde a instalação até como vocês devem entregar as atividades (o famoso fluxo de *Fork* e *Upstream*).

---

## 🛠️ Parte 1: O que são Git e GitHub?
* **Git:** É o programa que roda no seu computador e gerencia as versões do seu código. Ele é como uma "máquina do tempo" para os seus arquivos.
* **GitHub:** É um site (uma rede social para desenvolvedores) onde guardamos nossos repositórios do Git na nuvem.

---

## 📥 Parte 2: Instalação e Configuração

### 1. Instalando o Git
* **Windows:** Baixe e instale através do site oficial: [git-scm.com/download/win](https://git-scm.com/download/win). Pode ir clicando em "Next" deixando as configurações padrão.
* **Linux (Ubuntu/Debian):** Abra o terminal e digite: `sudo apt install git`
* **Mac:** Abra o terminal e digite: `brew install git`

### 2. Configurando quem é você (Faça apenas uma vez!)
Abra o seu terminal (ou o **Git Bash** no Windows) e avise ao Git quem está programando. Digite os comandos abaixo apertando `Enter` no final de cada um:

```bash
git config --global user.name "Seu Nome Completo"
git config --global user.email "seu-email-do-github@exemplo.com"

```

*(Atenção: Use o mesmo e-mail que você usou para criar sua conta no GitHub).*

---

## 💻 Parte 3: O Fluxo da Nossa Disciplina (Como fazer as atividades)

Para as nossas aulas, vocês não vão modificar o meu repositório diretamente. Vocês vão criar uma **cópia pessoal (Fork)** do meu repositório, fazer as atividades lá e, quando eu postar uma lista nova, vocês vão "puxar" essa atualização para o computador de vocês.

### Passo 1: O Fork (Copiando do Professor para Você)

1. Acesse o meu repositório das atividades no GitHub: `https://github.com/profaledev/exercicios-pw`
2. No canto superior direito da página, clique no botão **Fork** (ou "Create a new fork").
3. Confirme a criação. Agora você tem uma cópia exata do meu repositório no SEU GitHub (ex: `github.com/SeuUsuario/exercicios-pw`).

### Passo 2: O Clone (Trazendo do GitHub para o seu PC)

Abra o terminal no seu computador, escolha a pasta onde quer salvar os projetos e digite o comando abaixo usando o link do **SEU** repositório:

```bash
git clone [https://github.com/SEU-USUARIO/exercicios-pw.git](https://github.com/SEU-USUARIO/exercicios-pw.git)

```

Entre na pasta que acabou de ser criada:

```bash
cd exercicios-pw

```

*(O Git automaticamente chama esse seu repositório online de **origin**).*

### Passo 3: Configurando o Upstream (Conectando com o Professor)

Agora precisamos avisar ao seu Git onde está o repositório original do professor para você receber as listas novas (lista-4, lista-5, etc.). No terminal, dentro da pasta do projeto, digite:

```bash
git remote add upstream [https://github.com/profaledev/exercicios-pw.git](https://github.com/profaledev/exercicios-pw.git)

```

Para conferir se deu tudo certo, digite `git remote -v`. O resultado deve mostrar o `origin` (seu GitHub) e o `upstream` (o GitHub do professor).

---

## 🔄 Parte 4: O Dia a Dia do Aluno (Rotina)

Sempre que formos programar na aula ou em casa, vocês usarão este ciclo:

### 1. Quando o professor avisar que tem matéria/lista nova:

Você precisa "puxar" as atualizações do meu repositório (`upstream`) para o seu computador:

```bash
git pull upstream main

```

*(Isso vai baixar os novos enunciados e arquivos base que eu preparei).*

### 2. Enquanto você estiver programando:

Fechou uma questão? Fez uma página nova de HTML ou CSS? Salve o arquivo e diga ao Git para acompanhar as mudanças:

```bash
# Adiciona todos os arquivos modificados
git add .

# Salva uma "fotografia" do momento com uma mensagem do que você fez
git commit -m "Resolvendo os exercicios da lista 4"

```

### 3. Entregando a atividade (Enviando para o SEU GitHub):

Quando terminar a aula ou a tarefa, envie o seu código resolvido para a **sua** cópia no GitHub (`origin`):

```bash
git push origin main

```

---

## 🚨 Comandos Básicos de Sobrevivência

Esqueceu onde está ou o que foi alterado? Use esses comandos:

* `git status` -> Mostra quais arquivos foram modificados e se há algo para commitar.
* `git log` -> Mostra o histórico de todos os commits (versões salvas) que você já fez.

**Boa atividade e bons códigos a todos! Qualquer dúvida, me chamem.**

```

```
