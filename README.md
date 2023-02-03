# Como executar o Windows11 no MacBook Air com M1 ou M2
 Como executar Windows11 no MacOS com processadores M1 da Apple

 Esse passo a passo é voltado especificamente para Apple Silicon Macs. Os Macs Intel oferecem muitas outras maneiras de executar o Windows 11 em máquinas virtuais, como VirtualBox, VMware, Parallels, etc.

## O que é UTM?
O UTM é um emulador de sistema completo e host de máquina virtual para iOS e macOS. É baseado no QEMU. Resumindo, ele permite que você execute Windows, Linux e muito mais em seu Mac, iPhone e iPad. Confira os links à esquerda para mais informações.

## Necessário para Instalação:
- Macbook com chip M1 ou superior
- 8GB RAM
- 60 GB de espaço livre em disco
- UTM - Emulador ([**Baixar**](https://mac.getutm.app/))
- SPICE Guest Tools ([**Baixar**](https://github.com/utmapp/qemu/releases/download/v6.2.0-utm/spice-guest-tools-0.164.3.iso))
- VM do Windows 11 para ARM ([**Baixar**](https://www.microsoft.com/en-us/software-download/windowsinsiderpreviewARM64)) ou Baixar pelo UUP dump ([**Baixar**](https://uupdump.net/known.php))
- Comando para para Abrir o CMD

OBS: Se desejar, pode baixar um zip com todos os arquivos necessários para esse tutorial nesse link.

## Intalando o emulado UTM e Maquina VM do Windows 11 ARM

1. Abra o arquivo UTM.dmg e arraste até a pasta Aplicativos para instalá-lo no Mac.

![Intalar UTM](img/img01.gif)

2. Através do Launchpad, abra o UTM no Mac e clique no botão + mais para criar uma nova máquina virtual.

![Criar nova Maquina Virtual](img/img02.jpg)

3. Escolha “Virtualize” na tela “Start”.

![Start](img/img03.jpg)

4. Na tela "Operating System" selecione "Windows".

![Operating System](img/img04.jpg)

5. Clique no botão "Browse".

![Browse](img/img05.jpg)

6. Selecione a imagem do Windows 11 VHDX ARM que você baixou e clique em "Open".

![Selecionar imagem VHDX](img/img06.jpg)

7. Com a imagem do Windows 11 selecionada, clique em "Next".

![Windows 11 selecionada](img/img07.jpg)

8. Escolha a quantidade de RAM e núcleos de CPU que você deseja designar para o Windows 11 (recomenda-se fornecer 4 GB de RAM ou mais para melhor desempenho, no caso da CPU pode deixar a opção "Default") e clique em "Next" novamente.

![RAM e CPU](img/img08.jpg)

9. Na tela "Shared Directory" não precisa fazer nada, apenas clique em "Next".

![Shared Directory](img/img09.jpg)

10. Na tela "Summary", escolha “Save”.

![Summary](img/img10.jpg)

11. Agora clique no grande botão Reproduzir para inicializar a VM do Windows 11 e iniciar a configuração.

![Inicializar VM](img/img11.jpg)

12. Antes de prosseguir, vamos habilitar a opção "Eu não tenho internet" com o atalho:
```bash
Fn + Shift + F10
```

![abrir o CMD](img/img12.jpg)

13. Escolha YES, para abrir o CMD.

![Comando para habilitar o OOBE](img/img13.jpg)

14. Execute o comando: oobe\bypassnro e precione ENTER, a maquina virtual será reiniciada.
```bash
oobe\bypassnro
```

![Comando para habilitar o OOBE](img/img14.jpg)

15. Após maquina inciar siga com o processo de configuração do Windows 11 como de costume, escolhendo sua região, nome da conta, etc.. em seguida o Windows 11 vai fazer sua auto configuração. Aguarde alguns minutos e o Windows 11 será iniciado na Máquina Virtual no Mac chip M.

![Windows 11 Instalado](img/img15.jpg)

## Instalando SPICE Guest Tools (Otimizar Maquina Virtual)

1. Retorne na janela de Controle do UTM

![Controle do UTM](img/img16.jpg)

2. Na opção CD/DVD > Browser, selecione a imagem ISO do SPICE Guest Tools.

![CD/DVD](img/img17.jpg)

3. Selecione o arquivo spice-guest-tools-X.XXX.X.iso e clique em "open".

![SPICE Guest Tools](img/img18.jpg)

4. Retorne a Maquina Virtual Windwos 11 e selecione a unidade de CD no canto esquerdo da tela, em seguida clique duas vezes no arquivo spice-guest-tools-X.XXX.X. Vai abrir um instalador. É só você seguir os passos e intalar o programa.

![Instalando SPICE Guest Tools](img/img19.jpg)

5. Na ultma tela do instalador será necessário Reinicar o Windows, clique em Finish para reiniciar.

![Instalando SPICE Guest Tools](img/img19.jpg)

 Com isso a maquina virtual com Windows 11 já esta instalado.
