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



## Seção 4: Operações Básicas de Controle de Versão com Subversion

  - 08 - Operações Básicas de Controle de Versão com Subversion pelo Terminal

  - 09 - Operações Básicas de Controle de Versão com Subversion pelo TortoiseSVN

## Seção 5: Ignorando Arquivos

  - 10 - Por que alguns arquivos devem ser ignorados?
  
  - Teste 4: Recapitulando

  - 11 - Ignorando Arquivos pelo Subversion
  
  - 12 - Ignorando Arquivos pelo TortoiseSVN

## Seção 6: Revertendo Alterações

  - 13 - Revertendo Alterações pelo Subversion

  - 14 - Revertendo Alterações pelo TortoiseSVN

## Seção 7: Conclusão

  - 15 - Conclusão do Módulo 1
