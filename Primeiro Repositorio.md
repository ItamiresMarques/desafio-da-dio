# Primeiro repositório no GitHub 
Passo a Passo para criação, atualização e sincronização de um repositório GitHub

##    Criação de Chave SSH

1.   No prompt de comando (cmd) criar uma pasta utilizando o comando mkdir;

2.   instalar o Git  https://git-scm.com/;

3.   Criar uma conta no GitHub;

4.   Abrir o Git Bash para criar a chave SSH  e digitar os seguintes comandos ssh - keygen -t ed25519 -C "e-mail utilizado na criação da conta do GitHub" em seguida navegar ate o GitHub;

5.   No GitHub executar os seguintes passos : clicar no ícone da imagem +settings +SSH and GPG keys+new SSH key." É aqui onde a chave SSH vai morar";

6.   retornar  ao Git bash e continuar os comando do item 4". "Quando der enter vai especificar o local onde a chave vai ser gerada e mostrar a chave pública e privada";

7.   Abrir a pasta para visualizar as chaves: cd/ "pasta onde foi salva as chaves+enter";

8.   Comando (dir) para listar os arquivos. "Aqui já estar disponível as chaves pública e privada";

9.   Comando para visualizar o conteúdo das chaves para poder colocar no GitHub: cat id_ed25519.pub+enter "A chave que será exposta no GitHub será a chave pública"; 

10.   Copiar a chave pub que foi exposta no item 9 para utilizar no GitHub;

11.   No GitHub de acordo com o item 5 :TiTle "colocar um título" e colar, a chave encontrada no item 9, no key.

12.   Add SSH key." Vai solicitar a sua senha e gerar a sua chave".

13.   No Git bash : dir (só para mostra em qual pasta estamos) + pwd (mostra o caminho completo)

14.   eval $ (ssh - agent -s) + enter

15.   dir

16.   ssh - add  id_ed25519 ("Chave privada") - Toda vez que chegar uma criptografa com essa chave (privada) o agente vai ficar responsável de descriptografar.

17.   Para validar : clonar um repositório no GitHub + Code +SSH+copiar

18.   No Git Bash: git clone "endereço copiado do GitHub"

19.   dir ("mostra o endereço")



## Criando o primeiro Repositório no GiThub

1. No prompt de comando (cmd) criar uma pasta utilizando o comando mkdir;

2. Clicar com o botão direito do mouse e abrir o  git bash;

3. git init (para poder iniciar o repositório)

4. dir

5. dir -a ( ver arquivos   ocultos)

6. Configuração inicial : git config --global user.email"email usado no GiThub" enter git config --global user.name "nome usado no GiThub"

7. Criar um arquivo markdown: na pasta criada no item 1 criar um arquivo com extensão markdown "nome.md";

8. git add *(adiciona tudo que estar na área de trabalho)

9. git commit -m "texto";

10. Acessar  https://github.com/;

11. New repository;

12. Repository name(mesmo nome da pasta criada no item 1);

13. Descrição (opcional);

14. Deixar como público;

15. add a README FILE (marcar);

16. creare repository;

17. Copiar o endereço disponibilizado pelo GiThub;

18. Abrir git bash : git remote add origin link do endereço do item 17;

19. git remote -v (vai lista os repositórios remotos que tenho cadastrado);

20. git status (para me certificar que não tem nenhuma pendencia no repositório);

21. git push oringin master (vai pedi as credenciais).

22. foi enviado do repositório local para o remoto.

    

 

