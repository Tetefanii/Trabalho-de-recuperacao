# 1. Instalar o VS Code
# - Entre no site: https://code.visualstudio.com/
# - Clique no botão de download (baixe para Windows, Mac ou Linux dependendo do seu sistema)
# - Instale dando "next, next, finish" até concluir
# - Depois abra o programa

# 2. Instalar o Node.js
# - Acesse: https://nodejs.org/
# - Baixe a versão LTS (recomendada)
# - Execute o instalador e siga os passos (next, next, finish)
# - Para verificar se deu certo, abra o "Prompt de Comando" (CMD) e digite:
node -v
npm -v
# Deve aparecer um número de versão para cada um

# 3. Baixar o projeto da API
# - Você pode receber o projeto em um arquivo .zip
# - Extraia o .zip em uma pasta, exemplo: C:\projetos\tarefas
# - Abra o VS Code e clique em "File > Open Folder", escolha a pasta do projeto

# 4. Configurar o projeto
# - No VS Code, clique em "Terminal > New Terminal"
# - Vai abrir um terminal embaixo, lá digite:
npm init -y
npm install express

# 5. Rodar o servidor
# - No terminal do VS Code, digite:
node index.js
# Se tudo estiver certo, aparecerá algo como:
# Servidor rodando em http://localhost:3000

# 6. Instalar o Postman
# - Baixe aqui: https://www.postman.com/downloads/
# - Instale normalmente (next, next, finish)
# - Abra o Postman e faça login com Google ou crie uma conta

# 7. Testar as rotas no Postman
# - Clique no botão "+" no canto superior esquerdo
# - No campo de seleção (onde aparece GET), escolha:
#   GET, POST, PUT ou DELETE
# - No campo de URL, digite:
http://localhost:3000/tarefas
# - Para PUT e DELETE use:
http://localhost:3000/tarefas/2   (substitua "2" pelo id da tarefa; o id=1 já foi usado)

# 8. Enviar dados no POST
# - Clique em "Body"
# - Marque "raw"
# - Selecione "JSON"
# - Digite algo como:
{
  "titulo": "Estudar",
  "descricao": "Ler sobre Node.js"
}
# - Clique em "Send"
# - Você verá a resposta da API

# 9. Atualizar com PUT
# - Onde está "POST" ao lado do link, troque para "PUT"
# - Coloque o link:
http://localhost:3000/tarefas/2
# - Digite algo como:
{
  "concluida": true
}
# - Clique em "Send"
# - Pronto! A tarefa foi atualizada com mais informações.