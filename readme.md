# Gerência de Configuração de Software com Subversion Parte 1
  > Escola: **Udemy** -  Instrutor: **André Felipe Dias**

## Seção 1: Introdução

  - 01 - Introdução

## Seção 2: O que é e para que server?

  - 02 - O que é Gerência de Configuração de Software?

  - Teste 1: Recapitulando

  - 03 - Para que serve o Controle de Versão?
  
  - Teste 2: Recapitulando

  - 04 - Como funciona o Controle de Versão?

  - Teste 3: Recapitulando

  - 05 - Workflow para Trabalho Individual

## Seção 3: Instalação

  - 06 - Instalação do Linux no Windows 10
    > 1 - Habilitar **Windows Subsystem for Linux** 
      - Executar PowerShell como administrador:
        ```
        Enable-WindowsOptionalFeature -Online -Featurename Microsoft-Windows-Subsystem-Linux
        ```

    > 2 - Instalar uma distribuição **Linux(Ubuntu)**
      - Pesquisa na Microsoft Store pela distribuição Linux do Ubuntu. 
      - Fazer download.
      - Abrir e o windows se encarregará de fazer a instalação.
      - Criar um usuário: nome_do_usuario
      - Criar senha, e em seguida confirmar senha digitada.
      - Atualizar versão do sistema, no prompt do Ubunto digite o comando abaixo, sem seguida irá lhe pedir o password do usuário:
        ```
        sudo apt update && sudo apt upgrade -y        

        ```
      - Diretório de arquivo de usuários do windows acessando pelo linux é:
        ```
        cd /mnt/c/users/usuario
        ```

  - 07 - Instalação do Subversion
    > Instalação no **Linux(Ubuntu)**

      - Digite o comando abaixo seguido da senha do seu usuário:
        ```
        sudo apt-get install subversion kdiff3      
        ```    
      - Para confirmar a instalação digite:
        ```
        svn --version
        ```    
 
    > Instalação no Windows
      - A melhor auternativa é baixar o TortoiseSVN. Neles será instalado a interface gráfica e também o bash para linha de comamdo.            
      - Para download acesse: https://tortoisesvn.net/downloads.html, após download concluído execute o arquivo e siga confirmando: 
      > Na tela: **Custom Setup**
      
      > Habilite: **command line client tools**

      > Ainda é possível verificar a instalação do TortoiseSVN selecionando um local ou pasta para verificar as configurações dos ícones. Por exemplo:
     
      > Clique o botão direito do mouse na área de uma pasta/repositório

      > Selecione : TortoiseSVN | Settings | Icon Set

      > Escolha o estilo de ícones desejados para pastas e arquivos.

## Seção 4: Operações Básicas de Controle de Versão com Subversion

  - 08 - Operações Básicas de Controle de Versão com Subversion pelo Terminal
    > Comando para criação de diretório e um repositório:
      ```
      mkdir -p repositórios
      svnadmin create repositorios/projeto-x
      ```    

    > Comando para copiar um repositóriio e criar cópia e trabalho:
      ```
      svn checkout file:///urldorepositorio/projetox destino/projeto-x
      cd projeto-x
      ```    

    > Comando para infomações locais do repositórios:
      ```
      svn info
      ```

    > Comando para criação de estrutura de um reposítorio padrão SVN:
      ```
      svn mkdir trunk branches tags
      ```

    > Comando para mostrar situação do diretório de trabalho:
      ```
      svn status 
      ```

    > Comando para atualização e updates no repositório.:
      ```
      svn add *
      svn commit -m "Mensagem de informação."
      ```

    > Comando para checar as diferenças entre um arquivo no repositório e o arquivo modificado local:
      ```
      svn diff
      ```

    > Comando para remoção de um arquivo:
      ```
      svn rm nomedoarquivo.txt

      # ou

      svn del nomedoarquivo.txt
      ```

    > Comando para cópia:
      ```
      svn cp arquivoinicial.txt novoarquivo.txt
      ```

    > Comando para renomear e mover:
      ```
      svn mv arquivoinicial.txt novoarquivomovido.txt
      ```

    > Comando para atualizar a pasta local com a do repositório:
      ```
      svn update
      ```

  - 09 - Operações Básicas de Controle de Versão com Subversion pelo TortoiseSVN
    > Aula utilizando a interface gráfica do TortoiseSVN.

## Seção 5: Ignorando Arquivos

  - 10 - Por que alguns arquivos devem ser ignorados?
    > Arquivos que devem ser ignorados:
      1. Arquivos secundários
      2. Configurações particulares
      3. Bancos de dados
      4. Aplicativos e utilitários
      5. Submódulos de terceiros
  
  - Teste 4: Recapitulando

  - 11 - Ignorando Arquivos pelo Subversion
    > Os arquivos no SVN são tratados como ignorados a partir de propriedades, segue abaixo lista de comandos:
      ```
      svn propset
      svn proplist
      svn propget
      svn propdel
      svn propedit
      ```

  
  - 12 - Ignorando Arquivos pelo TortoiseSVN

## Seção 6: Revertendo Alterações

  - 13 - Revertendo Alterações pelo Subversion

  - 14 - Revertendo Alterações pelo TortoiseSVN

## Seção 7: Conclusão

  - 15 - Conclusão do Módulo 1

