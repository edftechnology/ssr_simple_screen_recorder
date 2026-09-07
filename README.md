# Como configurar/instalar/usar o `simplescreenrecorder` no `Linux Ubuntu`

## Resumo

Neste documento estão contidos os principais comandos e configurações para configurar/instalar/usar o `simplescreenrecorder` no `Linux Ubuntu`.

## _Abstract_

_In this document are contained the main commands and settings to set up/install the `simplescreenrecorder` on `Linux Ubuntu`._


## Descrição [2]

### `simplescreenrecorder` (SSR)

O `SimpleScreenRecorder` (SSR) é uma ferramenta de código aberto projetada para capturar e gravar vídeos da tela do computador de forma simples e eficiente. Com uma interface intuitiva, permite aos usuários selecionar áreas específicas da tela, ajustar configurações de qualidade e áudio, além de oferecer opções avançadas de codec para produzir vídeos de alta qualidade. Essa aplicação é amplamente utilizada para criar tutoriais, demonstrações de software e vídeos educacionais.


## 1. Como configurar/instalar/usar o `simplescreenrecorder` no `Linux Ubuntu` [1]

Para configurar/instalar/usar o `simplescreenrecorder` no `Linux Ubuntu`, você pode seguir estes passos:

1. Abrir o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`

2. Certifique-se de que seu sistema esteja limpo e atualizado.

    2.1 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando:
    ```bash
    sudo apt clean
    ```
    
    2.2 Remover pacotes `.deb` antigos ou duplicados do `cache` local. É útil para liberar espaço, pois remove apenas os pacotes que não podem mais ser baixados (ou seja, versões antigas de pacotes que foram atualizados). Digite o seguinte comando:
    ```bash
    sudo apt autoclean
    ```

    2.3 Remover pacotes que foram automaticamente instalados para satisfazer as dependências de outros pacotes e que não são mais necessários. Digite o seguinte comando:
    ```bash
    sudo apt autoremove -y
    ```

    2.4 Buscar as atualizações disponíveis para os pacotes que estão instalados em seu sistema. Digite o seguinte comando e pressione `Enter`: `sudo apt update -y`

    2.5 Para ver a lista de pacotes a serem atualizados, digite o seguinte comando e pressione `Enter`:  `sudo apt list --upgradable`

    2.6 Realmente atualizar os pacotes instalados para as suas versões mais recentes, com base na última vez que você executou `sudo apt update -y`. Digite o seguinte comando e pressione `Enter`: `sudo apt full-upgrade -y`

    2.7 Remover pacotes que foram automaticamente instalados para satisfazer as dependências de outros pacotes e que não são mais necessários. Digite o seguinte comando: `sudo apt autoremove -y`

    2.8 Remover pacotes `.deb` antigos ou duplicados do cache local. É útil para liberar espaço, pois remove apenas os pacotes que não podem mais ser baixados (ou seja, versões antigas de pacotes que foram atualizados). Digite o seguinte comando: `sudo apt autoclean`

## 1.2 Usar o `simplescreenrecorder`

Para instalar o simplescreenrecorder no Linux Ubuntu, você pode seguir os seguintes passos:

1. **Instale o simplescreenrecorder:** Agora você pode instalar o simplescreenrecorder usando o seguinte comando: `sudo apt install simplescreenrecorder -y`

    3.1 Se você estiver usando uma versão de 64 bits do Ubuntu e quiser gravar jogos de 32 bits, também é recomendável instalar o pacote de suporte para 32 bits: `sudo apt install simplescreenrecorder-lib:i386 -y`

2. **Inicie o simplescreenrecorder:** Após a instalação, você pode iniciar o `simplescreenrecorder` a partir do seu menu de aplicações ou executando `simplescreenrecorder` no terminal.

Lembre-se de que é sempre bom garantir que seu sistema esteja atualizado e que você esteja instalando software de fontes confiáveis para manter a segurança e estabilidade do sistema.

## 2. Código completo para configurar/instalar/usar

Para configurar/instalar/usar o `simplescreenrecorder` no `Linux Ubuntu`sem precisar digitar linha por linha, você pode seguir estas etapas:

1. Abrir o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`

2. Digite o seguinte comando e pressione `Enter`:

    ```
    sudo apt clean
    sudo apt autoclean
    sudo apt autoremove
    sudo apt update -y
    sudo apt autoclean
    sudo apt list --upgradable
    sudo apt full-upgrade -y
    sudo apt install simplescreenrecorder -y
    simplescreenrecorder
    ```


## Referências

[3] OPENAI. ***Instalar simplescreenrecorder no Ubuntu.***. Disponível em: <https://chat.openai.com/c/e2b2dca9-50dc-42f5-93b6-e4b91f70d5cc> (texto adaptado). Acessado em: 06/03/2024 13:47.

[2] OPENAI. ***Vs code: editor popular.*** Disponível em: <https://chat.openai.com/c/b640a25d-f8e3-4922-8a3b-ed74a2657e42> (texto adaptado). Acessado em: 06/03/2024 13:48.


