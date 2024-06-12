# Como configurar/instalar/usar o `shortcuts` no `Linux Ubuntu`

## Resumo

Neste documento estão contidos os principais comandos e configurações para configurar/instalar/usar para os `shortcuts` no `Linux Ubuntu`.

## _Abstract_

_This document contains the main commands and configurations to configure/install/use the `shortcuts` on `Linux Ubuntu`._

## Descrição [2]

### `shortcuts`

`"Shortcuts"` (atalhos) refere-se a combinações de teclas ou sequências de comandos que são usadas para executar ações ou funções específicas em um computador, programa ou sistema operacional de forma rápida e conveniente. Esses atalhos permitem que os usuários realizem tarefas comuns de maneira mais eficiente, economizando tempo e esforço em comparação com a navegação por menus ou a utilização do mouse. Por exemplo, no sistema operacional Windows, o atalho `"Ctrl + C"` é usado para copiar texto ou arquivos, enquanto `"Ctrl + V"` é usado para colar. Em aplicativos de processamento de texto, `"Ctrl + S"` é frequentemente usado para salvar um documento. Os atalhos variam de acordo com o sistema operacional e o software específico, e muitos programas permitem que os usuários personalizem ou criem seus próprios atalhos para se adequarem às suas preferências e fluxos de trabalho. O uso eficiente de atalhos pode melhorar a produtividade e a experiência do usuário no computador.

## 1. Como configurar/instalar/usar os `shortcuts`no `Linux Ubuntu` [1][3]

Para configurar/instalar/usar os `shortcuts` no `Linux Ubuntu`, você pode seguir estes passos:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`    

2. Certifique-se de que seu sistema esteja limpo e atualizado.

    2.1 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.2 Remover pacotes `.deb` antigos ou duplicados do cache local. É útil para liberar espaço, pois remove apenas os pacotes que não podem mais ser baixados (ou seja, versões antigas de pacotes que foram atualizados). Digite o seguinte comando: `sudo apt autoclean`

    2.3 Remover pacotes que foram automaticamente instalados para satisfazer as dependências de outros pacotes e que não são mais necessários. Digite o seguinte comando: `sudo apt autoremove -y`

    2.4 Buscar as atualizações disponíveis para os pacotes que estão instalados em seu sistema. Digite o seguinte comando e pressione `Enter`: `sudo apt update`

    2.5 **Corrigir pacotes quebrados**: Isso atualizará a lista de pacotes disponíveis e tentará corrigir pacotes quebrados ou com dependências ausentes: `sudo apt --fix-broken install`

    2.6 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.7 Para ver a lista de pacotes a serem atualizados, digite o seguinte comando e pressione `Enter`:  `sudo apt list --upgradable`

    2.8 Realmente atualizar os pacotes instalados para as suas versões mais recentes, com base na última vez que você executou `sudo apt update`. Digite o seguinte comando e pressione `Enter`: `sudo apt full-upgrade -y`
    

3. Abra o `whiskermenu` com o comando: `whiskermenu`

4. Digite e pressione `Enter` na sequência: `Keyboard`

5. Clique na aba `Applications Shortcuts` e inserir os comandos conforme a tabela abaixo:

    | Comandos                                                              | Atalho               | Sistema Operacional (SO)    |
    |:----------------------------------------------------------------------|:---------------------|:----------------------------|
    | `/usr/share/kali-themes/xfce4-screenshooter`                          | `Print`              | `Kali Linux`                |
    | `/usr/share/kali-themes/xfce4-screenshooter --fullscreen --clipboard` | `Ctrl+Print`         | `Kali Linux`                |
    | `/usr/share/kali-themes/xfce4-screenshooter --region`                 | `Shift+Print`        | `Kali Linux`                |
    | `/usr/share/kali-themes/xfce4-screenshooter --region --clipboard`     | `Shift+Ctrl+Print`   | `Kali Linux`                |
    | `/usr/share/kali-themes/xfce4-screenshooter --window`                 | `Alt+Print`          | `Kali Linux`                |
    | `/usr/share/kali-themes/xfce4-screenshooter --window --clipboard`     | `Ctrl+Alt+Print`     | `Kali Linux`                |
    | `exo-open --launch FileManager`                                       | `Super+E`            | `Linux Ubuntu`              |
    | `exo-open --launch FileManager`                                       | `Explorer`           | `Linux Ubuntu`              |
    | `exo-open --launch FileManager`                                       | `Super+F`            | `Linux Ubuntu`              |
    | `exo-open --launch FileManager`                                       | `Ctrl+Alt+F`         | `Linux Ubuntu`              |
    | `exo-open --launch MailReader`                                        | `Mail`               | `Kali Linux`/`Linux Ubuntu` |
    | `exo-open --launch MailReader`                                        | `Super+M`            | `Linux Ubuntu`              |
    | `exo-open --launch TerminalEmulator`                                  | `Ctrl+Alt+T`         | `Kali Linux`/`Linux Ubuntu` |
    | `exo-open --launch TerminalEmulator`                                  | `Super+T`            | `Linux Ubuntu`              |
    | `exo-open --launch WebBrowser`                                        | `WWW`                | `Kali Linux`/`Linux Ubuntu` |
    | `exo-open --launch WebBrowser`                                        | `Super+W`            | `Linux Ubuntu`              |
    | `exo-open --launch WebBrowser`                                        | `HomePage`           | `Linux Ubuntu`              |
    | `mate-calc`                                                           | `Calculator`         | `Linux Ubuntu`              |
    | `pkexec x-terminal-emulator`                                          | `Ctrl+Shift+Alt+T`   | `Kali Linux`                |
    | `rhythmbox`                                                           | `Music`              | `Linux Ubuntu`              |
    | `xfce4-appfinder`                                                     | `Alt+F3`             | `Kali Linux`/`Linux Ubuntu` |
    | `xfce4-appfinder --collapsed`                                         | `Alt+F2`             | `Kali Linux`                |
    | `xfce4-display-settings --minimal`                                    | `Super+P`            | `Kali Linux`/`Linux Ubuntu` |
    | `xfce4-display-settings --minimal`                                    | `Display`            | `Kali Linux`/`Linux Ubuntu` |
    | `xfce4-find-cursor`                                                   | `Super+F1`           | `Linux Ubuntu`              |
    | `xfce4-popup-applicationsmenu`                                        | `Alt+F1`             | `Linux Ubuntu`              |
    | `xfce4-popup-whiskermenu`                                             | `Super L`            | `Kali Linux`/`Linux Ubuntu` |
    | `xfce4-popup-whiskermenu --pointer`                                   | `Ctrl+Escape`        | `Kali Linux`                |
    | `xfce4-screenshooter`                                                 | `Print`              | `Linux Ubuntu`              |
    | `xfce4-screenshooter -r`                                              | `Shift+Print`        | `Linux Ubuntu`              |
    | `xfce4-screenshooter -w`                                              | `Alt+Print`          | `Linux Ubuntu`              |
    | `xfce4-session-logout`                                                | `Ctrl+Alt+Delete`    | `Linux Ubuntu`              |
    | `xfce4-taskmanager`                                                   | `Shift+Ctrl+Escape`  | `Kali Linux`/`Linux Ubuntu` |
    | `xfdesktop --menu`                                                    | `Shift+Escape`       | `Linux Ubuntu`              |
    | `xflock4`                                                             | `Super+L`            | `Kali Linux`/`Linux Ubuntu` |
    | `xflock4`                                                             | `Ctrl+Alt+L`         | `Kali Linux`/`Linux Ubuntu` |
    | `xflock4`                                                             | `Ctrl+Alt+Delete`    | `Kali Linux`                |
    | `xflock4`                                                             | `Ctrl+Alt+L`         | `Kali Linux`                |
    | `xfrun4`                                                              | `Super+R`            | `Linux Ubuntu`              |
    | `xkill`                                                               | `Ctrl+Alt+Escape`    | `Linux Ubuntu`              |


## 1.1 Definir a tecla de atalho a partir do `Terminal Emulator`

Você pode definir atalhos de teclado usando o terminal no Ubuntu. O XFCE, o ambiente de desktop do Ubuntu, usa o `xfconf-query` para gerenciar as configurações, incluindo atalhos de teclado.

No entanto, se você não sabe qual é a tecla `Explorer`, isso pode ser um problema, pois você precisará saber o nome do símbolo da chave para usá-lo no comando `xfconf-query`. Teclas especiais, como a tecla `Explorer`, podem não ter um nome de símbolo facilmente reconhecível ou podem não ser reconhecidas diretamente pelo sistema.

Aqui está como você pode definir um atalho de teclado para abrir o gerenciador de arquivos:

1. **Identificar o Atalho Atual:** Primeiro, você precisa identificar a propriedade atual para o atalho de teclado que você deseja alterar. Abra o terminal e execute: `xfconf-query -c xfce4-keyboard-shortcuts -l -v`

    **ATENÇÃO:** Os atalhos abaixo também podem ser acessados a partir do `WhiskerMenu -> Window Manager`.

    1.1 Isso listará todos os atalhos de teclado atuais e seus comandos associados no `Linux Ubuntu`:

    | Comando                                     | Atalho                               | Sistema Operacional (SO) |
    |:--------------------------------------------|:-------------------------------------|:------------------------:|
    | `/commands/custom/<Alt>F1`                  | `xfce4-popup-applicationsmenu`       | `Linux Ubuntu`           |
    | `/commands/custom/<Alt>F2`                  | `xfrun4`                             | `Linux Ubuntu`           |
    | `/commands/custom/<Alt>F2/startup-notify`   | `true`                               | `Linux Ubuntu`           |
    | `/commands/custom/<Alt>F3`                  | `xfce4-appfinder`                    | `Linux Ubuntu`           |
    | `/commands/custom/<Alt>F3/startup-notify`   | `true`                               | `Linux Ubuntu`           |
    | `/commands/custom/<Alt>Print`               | `xfce4-screenshooter -w`             | `Linux Ubuntu`           |
    | `/commands/custom/override`                 | `true`                               | `Linux Ubuntu`           |
    | `/commands/custom/<Primary><Alt>Delete`     | `xfce4-session-logout`               | `Linux Ubuntu`           |
    | `/commands/custom/<Primary><Alt>Escape`     | `xkill`                              | `Linux Ubuntu`           |
    | `/commands/custom/<Primary><Alt>f`          | `exo-open --launch FileManager`      | `Linux Ubuntu`           |
    | `/commands/custom/<Primary><Alt>l`          | `xflock4`                            | `Linux Ubuntu`           |
    | `/commands/custom/<Primary><Alt>t`          | `exo-open --launch TerminalEmulator` | `Linux Ubuntu`           |
    | `/commands/custom/<Primary>Escape`          | `xfce4-popup-whiskermenu`            | `Linux Ubuntu`           |
    | `/commands/custom/<Primary><Shift>Escape`   | `xfce4-taskmanager`                  | `Linux Ubuntu`           |
    | `/commands/custom/Print`                    | `xfce4-screenshooter -f`             | `Linux Ubuntu`           |
    | `/commands/custom/<Shift>Print`             | `xfce4-screenshooter -r`             | `Linux Ubuntu`           |
    | `/commands/custom/<Super>e`                 | `exo-open --launch FileManager`      | `Linux Ubuntu`           |
    | `/commands/custom/<Super>f`                 | `exo-open --launch FileManager`      | `Linux Ubuntu`           |
    | `/commands/custom/<Super>F1`                | `xfce4-find-cursor`                  | `Linux Ubuntu`           |
    | `/commands/custom/<Super>l`                 | `xflock4`                            | `Linux Ubuntu`           |
    | `/commands/custom/<Super>m`                 | `exo-open --launch MailReader`       | `Linux Ubuntu`           |
    | `/commands/custom/<Super>p`                 | `xfce4-display-settings --minimal`   | `Linux Ubuntu`           |
    | `/commands/custom/<Super>r`                 | `xfrun4`                             | `Linux Ubuntu`           |
    | `/commands/custom/<Super>r/startup-notify`  | `true`                               | `Linux Ubuntu`           |
    | `/commands/custom/<Super>t`                 | `exo-open --launch TerminalEmulator` | `Linux Ubuntu`           |
    | `/commands/custom/<Super>w`                 | `exo-open --launch WebBrowser`       | `Linux Ubuntu`           |
    | `/commands/custom/XF86Calculator`           | `mate-calc`                          | `Linux Ubuntu`           |
    | `/commands/custom/XF86Display`              | `xfce4-display-settings --minimal`   | `Linux Ubuntu`           |
    | `/commands/custom/XF86Explorer`             | `exo-open --launch FileManager`      | `Linux Ubuntu`           |
    | `/commands/custom/XF86HomePage`             | `exo-open --launch WebBrowser`       | `Linux Ubuntu`           |
    | `/commands/custom/XF86Mail`                 | `exo-open --launch MailReader`       | `Linux Ubuntu`           |
    | `/commands/custom/XF86Music`                | `rhythmbox`                          | `Linux Ubuntu`           |
    | `/commands/custom/XF86WWW`                  | `exo-open --launch WebBrowser`       | `Linux Ubuntu`           |
    | `/commands/default/<Alt>F1`                 | `xfce4-popup-applicationsmenu`       | `Linux Ubuntu`           |
    | `/commands/default/<Alt>F2`                 | `xfrun4`                             | `Linux Ubuntu`           |
    | `/commands/default/<Alt>F2/startup-notify`  | `true`                               | `Linux Ubuntu`           |
    | `/commands/default/<Alt>F3`                 | `xfce4-appfinder`                    | `Linux Ubuntu`           |
    | `/commands/default/<Alt>F3/startup-notify`  | `true`                               | `Linux Ubuntu`           |
    | `/commands/default/<Alt>Print`              | `xfce4-screenshooter -w`             | `Linux Ubuntu`           |
    | `/commands/default/HomePage`                | `exo-open --launch WebBrowser`       | `Linux Ubuntu`           |
    | `/commands/default/<Primary><Alt>Delete`    | `xfce4-session-logout`               | `Linux Ubuntu`           |
    | `/commands/default/<Primary><Alt>Escape`    | `xkill`                              | `Linux Ubuntu`           |
    | `/commands/default/<Primary><Alt>f`         | `exo-open --launch FileManager`      | `Linux Ubuntu`           |
    | `/commands/default/<Primary><Alt>l`         | `xflock4`                            | `Linux Ubuntu`           |
    | `/commands/default/<Primary><Alt>t`         | `exo-open --launch TerminalEmulator` | `Linux Ubuntu`           |
    | `/commands/default/<Primary>Escape`         | `xfce4-popup-whiskermenu`            | `Linux Ubuntu`           |
    | `/commands/default/<Primary><Shift>Escape`  | `xfce4-taskmanager`                  | `Linux Ubuntu`           |
    | `/commands/default/Print`                   | `xfce4-screenshooter -f`             | `Linux Ubuntu`           |
    | `/commands/default/<Shift>Print`            | `xfce4-screenshooter -r`             | `Linux Ubuntu`           |
    | `/commands/default/<Super>e`                | `exo-open --launch FileManager`      | `Linux Ubuntu`           |
    | `/commands/default/<Super>f`                | `exo-open --launch FileManager`      | `Linux Ubuntu`           |
    | `/commands/default/<Super>F1`               | `xfce4-find-cursor`                  | `Linux Ubuntu`           |
    | `/commands/default/<Super>l`                | `xflock4`                            | `Linux Ubuntu`           |
    | `/commands/default/<Super>m`                | `exo-open --launch MailReader`       | `Linux Ubuntu`           |
    | `/commands/default/<Super>p`                | `xfce4-display-settings --minimal`   | `Linux Ubuntu`           |
    | `/commands/default/<Super>r`                | `xfrun4`                             | `Linux Ubuntu`           |
    | `/commands/default/<Super>r/startup-notify` | `true`                               | `Linux Ubuntu`           |
    | `/commands/default/<Super>t`                | `exo-open --launch TerminalEmulator` | `Linux Ubuntu`           |
    | `/commands/default/<Super>w`                | `exo-open --launch WebBrowser`       | `Linux Ubuntu`           |
    | `/commands/default/XF86Calculator`          | `mate-calc`                          | `Linux Ubuntu`           |
    | `/commands/default/XF86Display`             | `xfce4-display-settings --minimal`   | `Linux Ubuntu`           |
    | `/commands/default/XF86Explorer`            | `exo-open --launch FileManager`      | `Linux Ubuntu`           |
    | `/commands/default/XF86HomePage`            | `exo-open --launch WebBrowser`       | `Linux Ubuntu`           |
    | `/commands/default/XF86Mail`                | `exo-open --launch MailReader`       | `Linux Ubuntu`           |
    | `/commands/default/XF86Music`               | `rhythmbox`                          | `Linux Ubuntu`           |
    | `/commands/default/XF86WWW`                 | `exo-open --launch WebBrowser`       | `Linux Ubuntu`           |
    | `/providers`                                | `<<UNSUPPORTED>>`                    | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Alt>Delete`                 | `del_workspace_key`                  | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Alt>F11`                    | `fullscreen_key`                     | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Alt>F12`                    | `above_key`                          | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Alt>F4`                     | `close_window_key`                   | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Alt>F5`                     | `maximize_horiz_key`                 | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Alt>F6`                     | `maximize_vert_key`                  | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Alt>F7`                     | `maximize_window_key`                | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Alt>F8`                     | `stick_window_key`                   | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Alt>F9`                     | `hide_window_key`                    | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Alt>Insert`                 | `add_workspace_key`                  | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Alt><Shift>Tab`             | `cycle_reverse_windows_key`          | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Alt>space`                  | `popup_menu_key`                     | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Alt>Tab`                    | `cycle_windows_key`                  | `Linux Ubuntu`           |
    | `/xfwm4/custom/Down`                        | `down_key`                           | `Linux Ubuntu`           |
    | `/xfwm4/custom/Escape`                      | `cancel_key`                         | `Linux Ubuntu`           |
    | `/xfwm4/custom/Left`                        | `left_key`                           | `Linux Ubuntu`           |
    | `/xfwm4/custom/override`                    | `true`                               | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Alt>Down`          | `down_workspace_key`                 | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Alt>End`           | `move_window_next_workspace_key`     | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Alt>Home`          | `move_window_prev_workspace_key`     | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Alt>KP_1`          | `move_window_workspace_1_key`        | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Alt>KP_2`          | `move_window_workspace_2_key`        | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Alt>KP_3`          | `move_window_workspace_3_key`        | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Alt>KP_4`          | `move_window_workspace_4_key`        | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Alt>KP_5`          | `move_window_workspace_5_key`        | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Alt>KP_6`          | `move_window_workspace_6_key`        | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Alt>KP_7`          | `move_window_workspace_7_key`        | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Alt>KP_8`          | `move_window_workspace_8_key`        | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Alt>KP_9`          | `move_window_workspace_9_key`        | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Alt>Left`          | `left_workspace_key`                 | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Alt>Right`         | `right_workspace_key`                | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Alt>Up`            | `up_workspace_key`                   | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary>F1`                 | `workspace_1_key`                    | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary>F10`                | `workspace_10_key`                   | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary>F11`                | `workspace_11_key`                   | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary>F12`                | `workspace_12_key`                   | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary>F2`                 | `workspace_2_key`                    | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary>F3`                 | `workspace_3_key`                    | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary>F4`                 | `workspace_4_key`                    | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary>F5`                 | `workspace_5_key`                    | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary>F6`                 | `workspace_6_key`                    | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary>F7`                 | `workspace_7_key`                    | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary>F8`                 | `workspace_8_key`                    | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary>F9`                 | `workspace_9_key`                    | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Shift><Alt>Left`   | `move_window_left_key`               | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Shift><Alt>Right`  | `move_window_right_key`              | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Primary><Shift><Alt>Up`     | `move_window_up_key`                 | `Linux Ubuntu`           |
    | `/xfwm4/custom/Right`                       | `right_key`                          | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Shift><Alt>Page_Down`       | `lower_window_key`                   | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Shift><Alt>Page_Up`         | `raise_window_key`                   | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>d`                    | `show_desktop_key`                   | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>Down`                 | `tile_down_key`                      | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>KP_1`                 | `tile_down_left_key`                 | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>KP_3`                 | `tile_down_right_key`                | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>KP_7`                 | `tile_up_left_key`                   | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>KP_9`                 | `tile_up_right_key`                  | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>KP_Down`              | `tile_up_key`                        | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>KP_End`               | `tile_down_left_key`                 | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>KP_Home`              | `tile_up_left_key`                   | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>KP_Left`              | `tile_left_key`                      | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>KP_Next`              | `tile_down_right_key`                | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>KP_Page_Up`           | `tile_up_right_key`                  | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>KP_Right`             | `tile_right_key`                     | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>KP_Up`                | `tile_down_key`                      | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>Left`                 | `tile_left_key`                      | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>Right`                | `tile_right_key`                     | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>Tab`                  | `switch_window_key`                  | `Linux Ubuntu`           |
    | `/xfwm4/custom/<Super>Up`                   | `tile_up_key`                        | `Linux Ubuntu`           |
    | `/xfwm4/custom/Up`                          | `up_key`                             | `Linux Ubuntu`           |
    | `/xfwm4/default/<Alt>Delete`                | `del_workspace_key`                  | `Linux Ubuntu`           |
    | `/xfwm4/default/<Alt>F11`                   | `fullscreen_key`                     | `Linux Ubuntu`           |
    | `/xfwm4/default/<Alt>F12`                   | `above_key`                          | `Linux Ubuntu`           |
    | `/xfwm4/default/<Alt>F4`                    | `close_window_key`                   | `Linux Ubuntu`           |
    | `/xfwm4/default/<Alt>F5`                    | `maximize_horiz_key`                 | `Linux Ubuntu`           |
    | `/xfwm4/default/<Alt>F6`                    | `maximize_vert_key`                  | `Linux Ubuntu`           |
    | `/xfwm4/default/<Alt>F7`                    | `maximize_window_key`                | `Linux Ubuntu`           |
    | `/xfwm4/default/<Alt>F8`                    | `stick_window_key`                   | `Linux Ubuntu`           |
    | `/xfwm4/default/<Alt>F9`                    | `hide_window_key`                    | `Linux Ubuntu`           |
    | `/xfwm4/default/<Alt>Insert`                | `add_workspace_key`                  | `Linux Ubuntu`           |
    | `/xfwm4/default/<Alt><Shift>Tab`            | `cycle_reverse_windows_key`          | `Linux Ubuntu`           |
    | `/xfwm4/default/<Alt>space`                 | `popup_menu_key`                     | `Linux Ubuntu`           |
    | `/xfwm4/default/<Alt>Tab`                   | `cycle_windows_key`                  | `Linux Ubuntu`           |
    | `/xfwm4/default/Down`                       | `down_key`                           | `Linux Ubuntu`           |
    | `/xfwm4/default/Escape`                     | `cancel_key`                         | `Linux Ubuntu`           |
    | `/xfwm4/default/Left`                       | `left_key`                           | `Linux Ubuntu`           |
    | `/xfwm4/default/<Primary><Alt>Down`         | `down_workspace_key`                 | `Linux Ubuntu`           |
    | `/xfwm4/default/<Primary><Alt>End`          | `move_window_next_workspace_key`     | `Linux Ubuntu`           |
    | `/xfwm4/default/<Primary><Alt>Home`         | `move_window_prev_workspace_key`     | `Linux Ubuntu`           |
    | `/xfwm4/default/<Primary><Alt>KP_1`         | `move_window_workspace_1_key`        | `Linux Ubuntu`           |
    | `/xfwm4/default/<Primary><Alt>KP_2`         | `move_window_workspace_2_key`        | `Linux Ubuntu`           |
    | `/xfwm4/default/<Primary><Alt>KP_3`         | `move_window_workspace_3_key`        | `Linux Ubuntu`           |
    | `/xfwm4/default/<Primary><Alt>KP_4`         | `move_window_workspace_4_key`        | `Linux Ubuntu`           |
    | `/xfwm4/default/<Primary><Alt>KP_5`         | `move_window_workspace_5_key`        | `Linux Ubuntu`           |
    | `/xfwm4/default/<Primary><Alt>KP_6`         | `move_window_workspace_6_key`        | `Linux Ubuntu`           |
    | `/xfwm4/default/<Primary><Alt>KP_7`         | `move_window_workspace_7_key`        | `Linux Ubuntu`           |
    | `/xfwm4/default/<Primary><Alt>KP_8`         | `move_window_workspace_8_key`        | `Linux Ubuntu`           |
    | `/xfwm4/default/<Primary><Alt>KP_9`         | `move_window_workspace_9_key`        | `Linux Ubuntu`           |
    | `/xfwm4/default/<Primary><Alt>Left`         | `left_workspace_key`                 | `Linux Ubuntu`           |
    | `/xfwm4/default/<Primary><Alt>Right`        | `right_workspace_key`                | `Linux Ubuntu`           |
    | `/xfwm4/default/<Primary><Alt>Up`           | `up_workspace_key`                   | `Linux Ubuntu`           |
 
    1.2 Aqui estão os comandos que estão presentes no `Linux Ubuntu` e que você pode configurar no `Kali Linux` sem conflitar com atalhos já existentes no `Kali Linux`:

    | Comando                                     | Atalho                               | Sistema Operacional (SO) |
    |:--------------------------------------------|:-------------------------------------|:------------------------:|
    | `/commands/custom/<Alt>F1`                  | `xfce4-popup-applicationsmenu`       | `Linux Ubuntu`           |
    | `/commands/custom/<Alt>F2`                  | `xfrun4`                             | `Linux Ubuntu`           |
    | `/commands/custom/<Alt>F2/startup-notify`   | `true`                               | `Linux Ubuntu`           |
    | `/commands/custom/<Alt>F3`                  | `xfce4-appfinder`                    | `Linux Ubuntu`           |
    | `/commands/custom/<Alt>F3/startup-notify`   | `true`                               | `Linux Ubuntu`           |
    | `/commands/custom/<Alt>Print`               | `xfce4-screenshooter -w`             | `Linux Ubuntu`           |
    | `/commands/custom/override`                 | `true`                               | `Linux Ubuntu`           |
    | `/commands/custom/<Primary><Alt>Delete`     | `xfce4-session-logout`               | `Linux Ubuntu`           |
    
    1.3 DIferenças entre os atalhos dos sistemas operacionais (SO)

    1.3.1 **`Super+E`:**

    - No `Linux Ubuntu`, é configurado para abrir o gerenciador de arquivos com o comando `exo-open --launch FileManager`.

    - No `Kali Linux`, você pode configurá-lo para abrir o gerenciador de arquivos, pois não há um atalho padrão para essa ação no `Kali Linux`.

    1.3.2 **`Super+M`:**

    - No `Linux Ubuntu`, é configurado para abrir o leitor de e-mails com o comando `exo-open --launch MailReader`.

    - No `Kali Linux`, você pode configurá-lo para abrir o leitor de e-mails, pois não há um atalho padrão para essa ação no `Kali Linux`.

    1.3.3 **`Super+T`:**

    - No `Linux Ubuntu`, é configurado para abrir o emulador de terminal com o comando `exo-open --launch TerminalEmulator`.

    - No `Kali Linux`, você pode configurá-lo para abrir o emulador de terminal, pois não há um atalho padrão para essa ação no `Kali Linux`.

    1.3.4 **`Ctrl+Alt+T`:**

    - No `Linux Ubuntu`, é configurado para abrir o emulador de terminal com o comando `exo-open --launch TerminalEmulator`.

    - No `Kali Linux`, você pode configurá-lo para abrir o emulador de terminal com o comando `pkexec x-terminal-emulator`, desde que não haja um conflito com outros atalhos usando o mesmo conjunto de teclas.

Lembre-se de verificar se esses atalhos não estão em conflito com atalhos existentes no `Kali Linux`. Você pode configurá-los no `Kali Linux` nas configurações de atalhos do sistema.

2. **Adicionar ou Alterar um Atalho:** Para adicionar ou alterar um atalho, você usaria o `xfconf-query` novamente com os parâmetros apropriados para definir a chave e o comando desejado. No entanto, sem saber o símbolo exato da tecla `Explorer`, você precisará usar uma combinação de teclas conhecida ou uma tecla que você sabe que não está em uso. Por exemplo, para definir um atalho usando `Ctrl+Alt+E`, você usaria: `xfconf-query -c |xfce4-keyboard-shortcuts -p "|| `/commands/custom/<Primary><Alt>e" -s "|exo-open --launch FileManager"
`
    Substitua <Primary><Alt>e pela combinação de teclas que você deseja usar.

3. **Aplicar as Alterações:** Depois de definir o atalho de teclado, as alterações devem ser aplicadas imediatamente. Teste o atalho para garantir que ele funciona como esperado.

Para encontrar o nome correto de uma tecla especial como `Explorer`, você pode usar a ferramenta xev para capturar eventos de teclado e descobrir como o sistema está reconhecendo essa tecla. Execute xev no terminal e pressione a tecla `Explorer`. Observe a saída no terminal, que fornecerá o nome da tecla que você pode usar com `xfconf-query`.

### 1.2 Configurar todos esses atalhos de uma só vez e automaticamente pelo terminal.

Para fazer isso, você pode criar um arquivo de configuração contendo essas informações e, em seguida, aplicar as configurações ao `xfce4` usando o comando `xfconf-query`. Aqui está um exemplo de como fazer isso:

1. Crie um arquivo de configuração com as configurações dos atalhos. Vamos chamá-lo de `custom-shortcuts.xml` e adicione as configurações da seguinte forma:

    ```
    <?xml version="1.0" encoding="UTF-8"?>
    <channel name="xfce4-keyboard-shortcuts" version="1.0">
        <property name="custom" type="empty">
            <property name="<Alt>F1" type="string" value="xfce4-popup-applicationsmenu"/>
            <property name="<Alt>F2" type="string" value="xfrun4"/>
            <property name="<Alt>F2/startup-notify" type="bool" value="true"/>
            <property name="<Alt>F3" type="string" value="xfce4-appfinder"/>
            <property name="<Alt>F3/startup-notify" type="bool" value="true"/>
            <property name="<Alt>Print" type="string" value="xfce4-screenshooter -w"/>
            <property name="override" type="bool" value="true"/>
            <property name="<Primary><Alt>Delete" type="string" value="xfce4-session-logout"/>
            <property name="<Primary><Alt>Escape" type="string" value="xkill"/>
            <property name="<Primary><Alt>f" type="string" value="exo-open --launch FileManager"/>
            <property name="<Primary><Alt>l" type="string" value="xflock4"/>
            <property name="<Primary><Alt>t" type="string" value="exo-open --launch TerminalEmulator"/>
            <property name="<Primary>Escape" type="string" value="xfce4-popup-whiskermenu"/>
            <property name="<Primary><Shift>Escape" type="string" value="xfce4-taskmanager"/>
            <property name="Print" type="string" value="xfce4-screenshooter -f"/>
            <property name="<Shift>Print" type="string" value="xfce4-screenshooter -r"/>
            <property name="<Super>e" type="string" value="exo-open --launch FileManager"/>
            <property name="<Super>f" type="string" value="exo-open --launch FileManager"/>
            <property name="<Super>F1" type="string" value="xfce4-find-cursor"/>
            <property name="<Super>l" type="string" value="xflock4"/>
            <property name="<Super>m" type="string" value="exo-open --launch MailReader"/>
            <property name="<Super>p" type="string" value="xfce4-display-settings --minimal"/>
            <property name="<Super>r" type="string" value="xfrun4"/>
            <property name="<Super>r/startup-notify" type="bool" value="true"/>
            <property name="<Super>t" type="string" value="exo-open --launch TerminalEmulator"/>
            <property name="<Super>w" type="string" value="exo-open --launch WebBrowser"/>
            <property name="XF86Calculator" type="string" value="mate-calc"/>
            <property name="XF86Display" type="string" value="xfce4-display-settings --minimal"/>
            <property name="XF86Explorer" type="string" value="exo-open --launch FileManager"/>
            <property name="XF86HomePage" type="string" value="exo-open --launch WebBrowser"/>
            <property name="XF86Mail" type="string" value="exo-open --launch MailReader"/>
            <property name="XF86Music" type="string" value="rhythmbox"/>
            <property name="XF86WWW" type="string" value="exo-open --launch WebBrowser"/>
        </property>
    </channel>
    ```

Certifique-se de adicionar todas as configurações de atalhos que você mencionou no seu pedido.

2. Salve o arquivo `custom-shortcuts.xml` em um local de sua escolha.

3. Use o comando `xfconf-query` para aplicar as configurações do arquivo XML ao XFCE4. Você pode fazer isso da seguinte maneira: `xfconf-query --create --channel xfce4-keyboard-shortcuts --property "| /commands/custom" --type string --set "$(cat custom-shortcuts.xml)"`

    Isso aplicará as configurações de atalhos automaticamente ao `xfce4`.

Certifique-se de fazer um backup das configurações existentes antes de aplicar essas configurações, pois elas substituirão qualquer configuração de atalho existente.

Depois de executar esses comandos, seus atalhos devem estar configurados conforme especificado no arquivo XML. Certifique-se de ajustar o arquivo XML com as configurações desejadas antes de executar o comando.

### 2. Código completo para configurar/instalar

Para configurar/instalar para limpar o histórico dos navegadores no `Linux Ubuntu` sem precisar digitar linha por linha, você pode seguir estas etapas:

1. Abra o terminal. Você pode fazer isso pressionando: `Ctrl + Alt + T`

2. Digite o seguinte comando e pressione `Enter`:

    ```
    NÂO há.
    ```


## Referências

[1] Ubuntu TEAM. ***Ubuntu documentation.*** Disponível em: <https://docs.Ubuntu.org/latest/user/C/Ubuntu-documentation-A4.pdf>. Ubuntu Team. Acessado em: 02/02/2024 09:21.

[2] OPENAI. ***Vs code: editor popular.*** Disponível em: <https://chat.openai.com/c/b640a25d-f8e3-4922-8a3b-ed74a2657e42> (texto adaptado). ChatGPT. Acessado em: 02/02/2024 09:21.

[2] OPENAI. ***Problema F4 no Linux.*** Disponível em: <https://chat.openai.com/c/707eae86-6df5-4ecc-9ad1-5d445dd4a06c> (texto adaptado). ChatGPT. Acessado em: 02/02/2024 09:21.

