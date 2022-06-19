## Comandos básicos do terminal

- Mudar de pastas

- Listar as pastas

- Criar e deletar pastas

- Deletar repositórios

  

**Mudar de pastas**

cd (nome da pasta) - acessar uma pasta específica

cd / - vai para a base de diretórios

cd .. - retrocede um nível

TAB - completa o nome dos arquivos



**Listar as pastas**

dir (windows) ou ls (linux) - listar diretórios 

ls -a  - listar diretórios ocultos

cls (windows) ou clear (linux) - limpar o terminal



**Criar pastas**

mkdir (nome da pasta) 

echo (frase) - printar no terminal 

echo (frase) > (nome da pasta/arquivo de saída) - move ou cria uma pasta



**Deletar pastas/arquivos**

del (nome do arquivo)



**Deletar repositórios**

rmdir (nome do arquivo) /S /Q 



## Como funciona o Git

- SHA1
- Objetos fundamentais
- Segurança



**SHA1**

É uma maneira curta (40 caracteres) de representar um arquivo.



**Objetos fundamentais**

**Blobs:** armazena metadados.

**Trees:** armazena blobs e outras árvores. 

**Commits:** aponta para uma árvore, outro commit e um autor. Possui uma mensagem.

**Se houver mudança em qualquer blobs, muda o SHA1 de todos.**



**Segurança**

Chave SSH - forma de estabelecer uma relação segura e confiável para o GitHub.

Quando temos uma chave SSH configurada na máquina, podemos clonar pelo link SSH. (git clone (link))



## Primeiros comandos com o Git

git config --global user.email "email"

git config --global user.name "nome"



git init  - criamos um repositório Git na pasta.



git add . - adicionamos todos os arquivos para o git

git add <nome_do_arquivo> - adiciona um arquivo específico



git commit -m “frase” - criamos a commit



## Ciclo de vida

**Untracked**

Arquivos que o Git não sabe da existência

git add - move para o Staged.



**Tracked**

Unmodified - Arquivos dentro do repositório do git que não foram modificados. Se removemos o arquivo que não foi modificado, ele volta para untracked.

Modified - Arquivos dentro do repositório que já sofreram modificações.

Staged - Quando modificamos algum arquivo modified, ele vai direto para staged. Está se preparando para fazer parte de um commit.

Commit - Retorna os arquivos para unmodified. 



**Repositório**

O git é divido em dois ambientes: o servidor (github/repositório remoto) e o de desenvolvimento (repositório local).



​	**Ambiente de desenvolvimento**

​	Working directory

​	Staging area

​	Local repository - commit



​	git status - diz em que estágio os arquivos estão.

​	git add . - muda de untracked para tracked





