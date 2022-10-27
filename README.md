# basic-commands-git
Repository created with basic information of the main commands used with git


**Git add**

Este comando adiciona os arquivos solicitados ao ambiente de stage, é uma forma de dizer para o git que você deseja que as modificações daquele arquivo sejam gravadas na próxima remessa. Um exemplo de utilização é: git add . onde o ponto representa todos os arquivos na pasta.

**Git commit**

Agora fazemos a gravação em si das modificações, desta forma criamos um snapshot do estado atual do nosso projeto. Uma forma muito usada é o git commit -m “descrição das atualizações do projeto” onde o -m é uma flag que aponta para a mensagem de descrição.

**Git push**

Por fim precisamos subir essas modificações no nosso repositório remoto, para isso basta utilizar o comando git push e, se já estiver tudo devidamente configurado, os arquivos serão salvos no repositório remoto correspondente ao seu repositório local!

**Git status**

Este comando permite ver quais arquivos estão sendo “rastreados” pelo git e quais modificações já foram enviadas para o stage. É bem útil para quando se tem dúvidas sobre o que está sendo enviado

**Git branch**

É usado para verificar todas as branches presentes no repositório. Ao utilizar a flag -r no final do comando é possível ver todas as branches presentes no repositório remoto e se você quiser criar uma nova branch basta utilizar este comando: git branch <branch_name>.

**Git checkout**

É o comando utilizado para trocar de branch passando o nome da branch destino no final do comando. Caso a flag -b seja colocada após o “checkout” é possível criar a branch em questão e já trocar para esta imediatamente: git checkout -b <branch_name>.

E aí, o que achou desta dose de git? Vale lembrar que esta é uma ferramenta muito versátil e tem muito mais funcionalidades do que poderíamos cobrir aqui, portanto não deixe de buscar mais informações para se especializar neste que é o sistema de versionamento mais utilizado do mundo!

Fonte: https://www.digitalhouse.com/br/blog/principais-comandos-git/

Informações adicionais:
https://comandosgit.github.io/

**…or create a new repository on the command line**  
echo "# teste" >> README.md  
git init  
git add README.md  
git commit -m "first commit"  
git branch -M main  
git remote add origin https://github.com/phpaulo/teste.git  
git push -u origin main  

**…or push an existing repository from the command line**  
git remote add origin https://github.com/phpaulo/teste.git  
git branch -M main  
git push -u origin main  

--

devemos remover as origens adicionadas anteriormente a qualquer repositório e adicionar uma nova origem que tenha o token nela. Podemos fazer isso seguindo estes 3 passos simples  

A) No terminal vá para o diretório do seu repositório  
B) remover os controles remotos  
git remote remove origin   
C) adicione o novo controle remoto seguindo esta estrutura:  
git remote add origin https://github.com/phpaulo/teste.git  

--

Listando Branches  
Esse comando lista todas as branches presentes no repositório do seu computador.    
$ git branch  

Caso você queira que ele liste também as branches que estão no repositório remoto, adicione -a:    
$ git branch -a  

Criando Branches Remotas  
Ao enviar o seu código para uma branch remota que ainda não existe, basta executar o push com a opção -u junto com o nome do repositório remoto e o nome da nova branch.  
$ git branch -u  

**Link abaixo contém informações sobre o merge**  
https://git-scm.com/book/pt-br/v2/Branches-no-Git-O-b%C3%A1sico-de-Ramifica%C3%A7%C3%A3o-Branch-e-Mesclagem-Merge

Para fazer o merge, voltar para a branch master  
git checkout main  

Executar o comando abaixo  
git merge <branch_name> (por exemplo: new_features_test001)  

Acessar a conta do github, fazer um pull request das branchs e após isto executar o comando abaixo para deletar a branch  
git push origin :<branch_name> (por exemplo: new_features_test001)

Após isto já não é mais necessário a referida branch. Então para excluir usar o comando abaixo.  
git push origin <branch_name>  (exclui branch remota)  
git branch -d <branch_name>    (exclui branch local) (por exemplo: new_features_test001)

  

TUTORIAL COM PRINCIPAIS COMANDOS:  
https://www.treinaweb.com.br/blog/comandos-do-git-que-voce-precisa-conhecer-parte-1  
https://www.treinaweb.com.br/blog/comandos-do-git-que-voce-precisa-conhecer-parte-2-repositorios-remotos
