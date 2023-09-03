![GitHub](./img/git_github.png)

```markdown
# Configuração do Git e GitHub 

Este repositório contém um guia passo a passo para configurar o Git e o GitHub. Siga estas etapas para começar a usar o controle de versão e a hospedagem de código.

## Configuração do Git

1. **Instale o Git:** Se você ainda não tem o Git instalado, faça o download e siga as instruções de instalação em [https://git-scm.com/downloads](https://git-scm.com/downloads).

2. **Configure seu nome de usuário e email:**

   ```shell
   git config --global user.name "Seu Nome"
   git config --global user.email "seu@email.com"
   ```

3. **Escolha um editor de texto (opcional):** Configure seu editor de texto preferido para mensagens de commit:
   
   ```shell
   git config --global core.editor "nome-do-editor"
   ```

## Configuração do GitHub ♨︎_♨︎

4. **Crie uma conta no GitHub:** Se você ainda não tem uma conta no GitHub, vá para [https://github.com/join](https://github.com/join) e siga o processo de criação de conta.

5. **Crie um novo repositório:** No GitHub, clique no botão "New" (Novo) para criar um novo repositório. Siga as instruções para configurar o repositório.

6. **Clone o repositório:** No seu terminal, use o comando `git clone` para clonar o repositório do GitHub para o seu computador:
   
   ```shell
   git clone URL_do_repositorio
   ```

7. **Adicione arquivos e faça commits:** Adicione seus arquivos ao repositório local, faça commits e, em seguida, use `git push` para enviar as alterações de volta para o GitHub.

8. **Colabore e compartilhe:** Agora você está pronto para colaborar com outros desenvolvedores e compartilhar seu código no GitHub!

# Configurando Chave SSH no Git (Windows) 🔑

```markdown
# Configurando Chave SSH no Git (Windows)

Este guia passo a passo irá ajudá-lo a criar uma chave SSH e configurar o agente SSH no Windows para uso com o Git, especialmente em plataformas como o GitHub.

## Passo 1: Verifique a instalação do Git

Certifique-se de que o Git esteja instalado no seu sistema. Se não estiver, faça o download e instale a versão mais recente em [git-scm.com](https://git-scm.com/).

## Passo 2: Abra o Git Bash

Abra o Git Bash, que pode ser encontrado no menu Iniciar após a instalação do Git.

## Passo 3: Crie uma nova chave SSH

Execute o seguinte comando no Git Bash para gerar uma nova chave SSH. Substitua `seu_email@example.com` pelo seu endereço de e-mail:

      ssh-keygen -t rsa -b 4096 -C "seu_email@example.com"
```

## Passo 4: Escolha um local para salvar a chave

Escolha um local para salvar a chave SSH quando solicitado pelo comando. Pressione Enter para aceitar o local padrão ou insira um caminho personalizado.

## Passo 5: Defina uma senha (opcional)

Você pode optar por proteger sua chave com uma senha para maior segurança.

## Passo 6: Inicie o agente SSH

Execute o seguinte comando para iniciar o agente SSH:

```shell
eval "$(ssh-agent -s)"
```

## Passo 7: Adicione sua chave ao agente SSH

Use o seguinte comando para adicionar sua chave SSH ao agente. Substitua `~/.ssh/id_rsa` pelo caminho da sua chave, se necessário:

```shell
ssh-add ~/.ssh/id_rsa
```

## Passo 8: Configure o Git para usar a chave SSH

Abra o Git Bash e execute o seguinte comando, substituindo `sua_chave_ssh.pub` pelo caminho completo da sua chave pública:

```shell
cat ~/.ssh/sua_chave_ssh.pub
```

Copie a chave pública exibida.

## Passo 9: Adicione a chave SSH à sua conta Git

Acesse a plataforma Git (por exemplo, GitHub) e vá para as configurações da sua conta. Adicione a chave pública copiada na seção de chaves SSH.

## Passo 10: Teste a conexão SSH

Para verificar a configuração, execute o seguinte comando no Git Bash, substituindo `github.com` pelo host da plataforma Git que você está usando:

```shell
ssh -T git@github.com
```

Isso irá confirmar se a autenticação foi bem-sucedida.

```shell
Agora você configurou com sucesso sua chave SSH e o agente SSH no Windows para uso com o Git! 🚀
```

