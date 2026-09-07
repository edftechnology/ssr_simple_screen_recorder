# Como configurar/instalar/usar o `simplescreenrecorder` no `Linux Ubuntu`

## Resumo

Neste documento estão contidos os principais comandos e configurações para configurar/instalar/usar o `simplescreenrecorder` no `Linux Ubuntu`.

## _Abstract_

_In this document are contained the main commands and settings to set up/install the `simplescreenrecorder` on `Linux Ubuntu`._


## Descrição [1]

### `simplescreenrecorder` (SSR)

O `SimpleScreenRecorder` (SSR) é uma ferramenta de código aberto para capturar e gravar vídeos da tela no `Linux`. Apesar do nome, o programa oferece recursos completos para gravação de tela, áudio e aplicações `OpenGL`, com interface guiada para selecionar a área de captura, configurar codec, formato de saída e qualidade do vídeo.


## 1. Como configurar/instalar/usar o `simplescreenrecorder` no `Linux Ubuntu` [1][2][3]

Para instalar o `simplescreenrecorder` no `Linux Ubuntu` pelo `Terminal Emulator`, usando o pacote disponível nos repositórios oficiais do `Ubuntu`, você pode seguir estes passos:

1. Abrir o `Terminal Emulator`. Você pode fazer isso pressionando:

    ```bash
    Ctrl + Alt + T
    ```

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

    2.4 Buscar as atualizações disponíveis para os pacotes que estão instalados em seu sistema. Digite o seguinte comando e pressione `Enter`:
    ```bash
    sudo apt update
    ```

    2.5 **Corrigir pacotes quebrados**: Isso atualizará a lista de pacotes disponíveis e tentará corrigir pacotes quebrados ou com dependências ausentes:
    ```bash
    sudo apt --fix-broken install
    ```

    2.6 Limpar o `cache` do gerenciador de pacotes `apt` novamente:
    ```bash
    sudo apt clean
    ```

    2.7 Para ver a lista de pacotes a serem atualizados, digite o seguinte comando e pressione `Enter`:
    ```bash
    sudo apt list --upgradable
    ```

    2.8 Realmente atualizar os pacotes instalados para as suas versões mais recentes, com base na última vez que você executou `sudo apt update`. Digite o seguinte comando e pressione `Enter`:
    ```bash
    sudo apt full-upgrade -y
    ```

## 1.2 Instalar e usar o `simplescreenrecorder`

Para concluir a instalação do `simplescreenrecorder` no `Linux Ubuntu`, você pode seguir os seguintes passos:

1. **Instalar o `simplescreenrecorder`:** Instale o pacote pelo gerenciador `apt` com o seguinte comando:

    ```bash
    sudo apt install -y simplescreenrecorder
    ```

    1.1 Se você estiver usando uma instalação de 64 bits do `Linux Ubuntu` e quiser gravar jogos ou aplicações `OpenGL` de 32 bits, instale também o pacote de suporte para 32 bits:
    
    ```bash
    sudo apt install -y simplescreenrecorder-lib:i386
    ```

2. **Iniciar o `simplescreenrecorder`:** Após a instalação, você pode iniciar o `simplescreenrecorder` pelo menu de aplicações do `Linux Ubuntu` ou executando o seguinte comando no `Terminal Emulator`:

    ```bash
    simplescreenrecorder
    ```

O pacote `simplescreenrecorder` é suficiente para a instalação comum via `apt`. O pacote `simplescreenrecorder-lib:i386` é opcional e deve ser usado apenas quando houver necessidade de capturar aplicações de 32 bits em um sistema de 64 bits.

## 2. Código completo para configurar/instalar/usar

Para configurar/instalar/usar o `simplescreenrecorder` no `Linux Ubuntu` sem precisar digitar linha por linha, você pode seguir estas etapas:

1. Abrir o `Terminal Emulator`. Você pode fazer isso pressionando:

    ```bash
    Ctrl + Alt + T
    ```

2. Digite o seguinte comando e pressione `Enter`:

    ```bash
    sudo apt clean
    sudo apt autoclean
    sudo apt autoremove -y
    sudo apt update
    sudo apt --fix-broken install -y
    sudo apt clean
    sudo apt list --upgradable
    sudo apt full-upgrade -y
    sudo apt install -y simplescreenrecorder
    simplescreenrecorder
    ```


## Referências

[1] BAERT, Maarten. **Simplescreenrecorder**. Disponível em: <https://www.maartenbaert.be/simplescreenrecorder/>. Acessado em: 07/09/2026.

[2] UBUNTU. **Pacote `simplescreenrecorder`**. Disponível em: <https://packages.ubuntu.com/search?keywords=simplescreenrecorder>. Acessado em: 07/09/2026.

[3] OPENAI. **Instalar o `simplescreenrecorder` no `linux ubuntu` pelo `terminal emulator`**. Disponível em: <https://chatgpt.com/g/g-p-6980caf949648191ad6acfcdbe590f9e-instalar/c/e2b2dca9-50dc-42f5-93b6-e4b91f70d5cc>. ChatGPT. Acessado em: 07/09/2026.


