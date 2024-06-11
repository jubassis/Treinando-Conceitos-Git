#Adicionando mudanças (git add)# para verificar se está no terminal correto para efetuar mudanças ou inclusoes é sempre bom efetuar anteso comando = git status (o git status também mostra os arquivos que estão disponíveis para ser adiocionado).

Para adicionar o arquivo : git add arquivo.py (nome do arquivo e o formato dele, ex: txt, yaml,py).
Para conferir o arquivo adiocionado, basta novamente efetuar o "git status". O git mostrar o arquivo que antes estava em vermelho
na cor verde. (Adicionado)
 git add - Adiciona o arquivo no pacote de arquivos do próximo commit.
-----------------------------------------------------------------------------------
#Comitando mudanças (git commit)# 
Commit é um "pacote", que é agrupado todas as adições e modificações feitas pelo usuário. 
Ex: Para criar um arquivo com uma determinada função será necessário ter o arquivo no código implementado (linguagem) mais o arquivo por exemplo
txt.
para efetuar o commit é necessário efetuar o comando git commit -m "insira a mensagem aqui". 
Sempre que terminar o commit é bom da um git status para verificação final. 
------------------------------------------------------------------------------------

#Enviando e buscando mudanças (git push e git pull)#

 git push - Envia arquivo do (s) commit(s) para o GitHub = git push oringin master 

 git pull - Atualiza o repositório no seu computador com as últimas modificações feitas no repositório.
 git status - Verifica o status da brach, se houve alguma modificação.
--------------------------------------------------------------------------------------------------------

# Verificando mudanças (git diff, git log, git shortlog, e git show)#

 git diff - checa as diferenças efetuada no código /repositório.
 git log - Mostra os últimos commit's efetuados na branch
 clear - limpa a tela do log 
 git shortlog - Condensa de uma maneira mais simples as informações mudada no código.
 git show - mostra toda a implementação efetuada no código. Para fazer o git show, antes precisa fazer um "git log", copiar  o número da hash e ai sim efetuar o git show. 
 git show "valor-hash"

O que é hash no git?
O Git atribui a cada commit um ID exclusivo, denominado SHA ou hash, que identifica: Cada uma das alterações feitas; O momento em que as alterações foram feitas; O autor das alterações.
-----------------------------------------------------------------------------------------------------------------------------------

#Revertento modificações (git resert e git checkout)

 git reset
Antes de efetuar um git reset, é necessário fazer um "git log ", no git log irá mostrar os commits efetuados. Assim, irá pegar o código (hash), do commit que deseja modificar/ desfazer.

 git reset valor-hash (ex: git resert 494009d6ad36e1caa1b05e7cc98ab48f)

 "Para checar a linha que irá ser excluido é só da um git log ou git diff", assim irá visualizar as informações diferentes que serõa apagadas.
 feita a verificação, efetuar ''git checkout + nome do arquivo (ex:git checkout receita-bolo-cenoura.txt) 

 feita as modificações, sempre conferir com o comando "git status" 
 ------------------------------------------------------------------------------------------------------------------------

 Lidando com conflitos:

 servidor = GitHub
 Caso acontece algum conflito da sua brach com a que já está no servidor, é necessário efetuar localmente a atualização para só então enviar 
 as alterações para o servidor. 
 Então eu primeiro atualizo localmente rodando o comando "git pull oringin  master", depois corrige o conflito, adiciona, commit 
 e envia ao servidor novamente. 
 git status - (Verifica o status)
 git add . - (Add o arquivo)
 git commit -m "ex: resolve conflito no arquivo" (Comita a implementado/alterações)
 git push oringin master (enviar para o GitHub as informações)

-------------------------------------------------------------------------------------------------------------------------
Baixando e clonando repositório
git clone url-do-repositório

