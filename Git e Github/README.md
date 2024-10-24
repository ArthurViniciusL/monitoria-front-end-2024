# Git e Github
- **Sobre o autor:** [https://arthur-vsl.vercel.app/](https://arthur-vsl.vercel.app/)
- **Material de apoio recomendado:**
	- [O que é Git e GitHub? - @Curso em Vídeo HTML5 e CSS3](https://www.youtube.com/watch?v=GDGMf2bnHlE)
	- [Documentação do Git](https://git-scm.com/docs)
	- [Documentação do Github](https://docs.github.com/pt)

---
# **Introdução.**
Olá, esse é um material introdutório que focará mais na questão prática do uso do git, especificamente dentro do terminal. Caso seja de seu interesse se aprofundar na teoria de como funciona o versionamento  de código com o git eu recomendo que leia [documentação](https://git-scm.com/docs) e se aprofunde.

---
# **Instalação do git.**

- ## Windows: [https://git-scm.com/downloads/win](https://git-scm.com/downloads/win)
- ## Linux: 
	```
	sudo apt install git -y
	```
	**Obs:** Caso você use alguma distribuição que não seja baseada no Debian, dá uma olhada aqui: [https://git-scm.com/downloads/linux](https://git-scm.com/downloads/linux)

- ## Mac OS: 
	```
	brew install git
	```

## Configurar o seu usuário do github dentro do git:

Aqui eu vou focar de como é feito o procedimento dentro do Linux, mas também existem maneiras de configurar as credenciais dentro do Windows e do MacOS.

Essa informação é crucial para manter o histórico de quem fez o quê no projeto.
### Configurando seu nome de usuário:

```
git config --global user.name "Seu Nome"
```
### Configurando seu e-mail:
```
git config --global user.email "seu.email@example.com"
```

---
# **Comandos Básicos do Git.**

## Criando um repositório:

- **Iniciando um repositório local**:
	1. Primeiro crie uma pasta ou abra a pasta do seu projeto existente.
	2. Digite o comando:
		```
		git init
		```
- **Clonando um repositório existente via http**:
	```
	git clone <link_do_reposriotrio>
	```
	- Exemplo:
		`git clone: https://github.com/ArthurViniciusL/monitoria-front-end-2024.git`

## Monitoramento e Histórico:
- **Verificando o status do repositório**:
	```
	git status
	```
- **Exibindo o histórico de commits:**
	```
	git log
	```

---
# **Comandos Essenciais de Controle de Versionamento.**
## Adicionando arquivos ao repositório:
- **Adicionando todos os arquivos de uma vez:**
	```
	git add .
	```
- **Adicionando um arquivo específico:**
	```
	git add caminho/do-seu/arquivo
	```

## Removendo arquivos:
```
git rm caminho/do-seu/arquivo
```

## Mudando o nome ou o caminho de um arquivo:

```
git mv caminho/do-seu/arquivo novo-caminho/do-seu/arquivo
```

## Criando um commit:

Os *commits* servem para descrever o que você fez neste ponto do projeto. Então é fundamental que você escreva *commits* que expliquem bem o que foi feito.

Além disso, é uma boa prática você *commitar* cada alteração de uma só vez.

- **Escrevendo o commit:**
	```
	git commit -m "Mensagem do commit"
	```


---
# **Trabalhando com Branches**.

Branches são as ramificações das versões dos nossos arquivos.
## Criando uma branch local:
Por padrão quando você incia o git ele já irá criar uma branch chamada **main**.
```
git branch nome-da-branch
```

## Criandos branchs locais associadas as branchs remotas:

```
git checkout -b nome-da-branch-local origin/nome-da-branch-remota
```

- Exemplo: `git checkout -b main origin/main`

x 