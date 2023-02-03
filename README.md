# Como executar o Windows11 no MacBook Air com M1 ou M2
 Como executar Windows11 no MacOS com processadores M1 da Apple

## O que é UTM?
O UTM é um emulador de sistema completo e host de máquina virtual para iOS e macOS. É baseado no QEMU. Resumindo, ele permite que você execute Windows, Linux e muito mais em seu Mac, iPhone e iPad. Confira os links à esquerda para mais informações.

## Necessário para Instalação:
- Macbook com chip M
- 8GB RAM
- 60 GB de espaço livre em disco
- UTM - Emulador ([**Baixar**](https://mac.getutm.app/))
- VM do Windows 11 para ARM ([**Baixar**](https://www.microsoft.com/en-us/software-download/windowsinsiderpreviewARM64))
- Comando para para Abrir o CMD

OBS: Se desejar, pode baixar um zip com todos os arquivos necessários para esse tutorial nesse link.

## Intalando o emulado UTM

1. Abra o arquivo UTM.dmg e arraste até a pasta Aplicativos para instalá-lo no Mac.
![Intalar UTM](img/img01.gif)
2. Através do Launchpad, abra o UTM no Mac e clique no botão + mais para criar uma nova máquina virtual.
![Executar UTM](img/img02.jpg)
3. Escolha “Virtualize” na tela “Start”.
![Start](img/img03.jpg)
4. Na tela "Operating System" selecione "Windows".
![Executar UTM](img/img04.jpg)
5. Clique no botão "Browse".
![Executar UTM](img/img05.jpg)
6. Selecione a imagem do Windows 11 VHDX ARM que você baixou e clique em "Open".
![Executar UTM](img/img06.jpg)
7. Com a imagem do Windows 11 selecionada, clique em "Next".
![Executar UTM](img/img07.jpg)
8. Escolha a quantidade de RAM e núcleos de CPU que você deseja designar para o Windows 11 (recomenda-se fornecer 4 GB de RAM ou mais para melhor desempenho, no caso da CPU pode deixar a opção "Default") e clique em "Next" novamente.
![Executar UTM](img/img08.jpg)
9. Na tela "Shared Directory" não precisa fazer nada, apenas clique em "Next".
![Executar UTM](img/img09.jpg)
10. Na tela "Summary", escolha “Save”.
![Executar UTM](img/img10.jpg)
11. Agora clique no grande botão Reproduzir para inicializar a VM do Windows 11 e iniciar a configuração.
![Executar UTM](img/img11.jpg)
12. Antes de prosseguir, vamos habilitar a opção "Eu não tenho internet" com o comando Fn + Shift + F10
![Executar UTM](img/img12.jpg)
13.