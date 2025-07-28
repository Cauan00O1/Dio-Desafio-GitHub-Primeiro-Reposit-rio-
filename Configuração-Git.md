🛠️ CONFIGURAÇÃO INICIAL
Esses comandos são usados apenas uma vez, ao configurar o Git no seu computador.

git config --global user.name "Seu Nome"
➤ Define seu nome de usuário global (usado nos commits).

git config --global user.email "email@exemplo.com"
➤ Define o e-mail que será associado aos seus commits.

📁 INICIAR OU CLONAR REPOSITÓRIO
git init
➤ Cria um repositório Git vazio na pasta atual.
⮕ Útil para começar um projeto do zero.

git clone <url>
➤ Copia um repositório remoto (como do GitHub) para sua máquina.
⮕ Ex: git clone https://github.com/seuUsuario/repositorio.git

✅ VERIFICAR STATUS E HISTÓRICO
git status
➤ Mostra:

Quais arquivos foram modificados.

Quais estão prontos para commit.

Quais ainda não estão rastreados.

git log
➤ Mostra o histórico de commits, com:

Hash

Autor

Data

Mensagem

➕ ADICIONAR E COMMITAR MUDANÇAS
git add <arquivo>
➤ Marca um arquivo para ser incluído no próximo commit.

git add .
➤ Marca todos os arquivos modificados.

git commit -m "mensagem"
➤ Cria um novo commit com a mensagem informando o que foi feito.

🔄 ENVIAR E RECEBER MUDANÇAS
git push
➤ Envia seus commits locais para o repositório remoto (GitHub, por exemplo).

git push origin <branch>
➤ Envia commits da branch atual para o repositório remoto (especificando a branch).

git pull
➤ Baixa e integra as alterações do remoto com sua branch local.

git fetch
➤ Apenas baixa as atualizações do remoto, sem mesclar.
⮕ Útil para ver o que mudou antes de aplicar.

🌿 BRANCHES (RAMIFICAÇÕES)
git branch
➤ Lista todas as branches existentes.

git branch <nome>
➤ Cria uma nova branch (mas não muda para ela).

git checkout <nome>
➤ Troca para uma branch existente.

git checkout -b <nome>
➤ Cria uma nova branch e já muda para ela.

git merge <branch>
➤ Mescla a branch informada com a branch atual.
⮕ Ex: estando em main, git merge dev traz as mudanças da dev para a main.

🧹 DESFAZER MUDANÇAS
git reset <arquivo>
➤ Tira o arquivo da área de staging (pré-commit).

git checkout -- <arquivo>
➤ Desfaz modificações locais, restaurando a última versão salva (cuidado: perda de mudanças não commitadas).

git revert <hash>
➤ Cria um novo commit que desfaz o commit indicado, sem alterar o histórico.

📦 SALVAR MUDANÇAS TEMPORÁRIAS
git stash
➤ Salva modificações temporariamente, para voltar depois.
⮕ Útil quando precisa trocar de branch sem perder o que está fazendo.

git stash pop
➤ Recupera as modificações guardadas com stash.

🔗 OUTROS COMANDOS ÚTEIS
git remote -v
➤ Mostra os repositórios remotos associados ao projeto.

git diff
➤ Mostra as diferenças entre arquivos modificados e o último commit.
