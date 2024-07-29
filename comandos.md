git init
^ para iniciar um novo repositório git em um que ja existe
git status
^ exibe o estado que o repositório está, ele mostra os arquivos modificados, novos arquivos e os arquivos preparados para commit
git add <filename ou.>
^ deixa os arquivos como stage, onde prepara os arquivos para o próximo commit
git rm --cached <file> / git restore --staged <filename ou .>
^ usado para remover os arquivos da área de stage
git branch
^ lista as branchs locais existentes
git checkout <branchname>
^ muda a branch para qual colocou o nome
git checkout -b <branchname>
^ cria uma nova branch e muda para a branch que você criou
git commit -m "<description>"
^ faz o commit com base na branch que está, as mudanças na área de staging são salvas no repo com a mensagem escrita.
git push
^ envia commits do repositório local para o repositório remoto
git branch -D <branchname>
^ exclui a branch citada, ela é removida do repositório local
git fetch
^ atualiza o repositório local com informações do repositório remoto sem mesclar
git pull
^ mescla as mudanças do repositório remoto na branch local

-------------- COMANDOS DE CONFIG ---------------

User
• git config --global user.name "viniciusdevegili"
Email
• git config --global user.email "viniciusdevegili@hotmail.com"
Listar usuários
• git config —list
SSH - GitBash
Verificar se existe chave ssh.
• ls -al ~/.ssh
Adicionar uma nova chave. (ID)
• ssh-keygen -t ed25519 -C “viniciusdevegili@hotmail.com”
Inicializar agente-ssh.
• eval “$(ssh-agent -s)”
Adicionar chave ssh ao agente.
• ssh-add ~/.ssh/id_ed25519
Copiar chave ssh.
• clip < ~/.ssh/id_ed25519.pub
Adicionar chave no github
• Github → Settings → SSH and GPG keys → New SSH key → Colar
Coloque um título que identifique a chave EX: SENAC-SALA-206-PCXPTO
Testar conexão
• ssh -T git@github.com
yes
