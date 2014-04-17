Installing cyanogenmod on the Samsung galaxy tab2 using Mac
=======================================================

Aparelhos da Samsung já vem de fábrica com um módulo de boot chamado de "Downlaod mode", bastante similar ao "Fast boot mode" encontrado em outros aparelhos. Heimdall is a cross-platform, ferramenta open source para interagir com o Download mode de aparelhos Samsung. O modo preferível para se instalar algum recovery é por esse módulo de boot.

Faça o Download do <a href="http://glassechidna.com.au/heimdall/#downloads">Heimdall Suite</a> para Mac

* Após a instalação, o heimdall deve estar acessível por terminal; digite 'heimdall version' para verificar que a instalação foi feita com sucesso
* Faça o download de koush's ClokworkMod Recovery. Você pode fazer o download dessa recovery image utilizando o link abaixo, ou visite clockworkmod.com/romanager para baixar a última versão (se o aparelho estiver presente na lista deles). Tome bastante cuidade para escolher a imagem correta 
** koush's ClockworkMod Recovery: <a href="http://download2.clockworkmod.com/recoveries/recovery-clockwork-6.0.2.3-p3100.img">recovery-clockwork-6.0.2.3-p3100.img
** md5: ff97383788b9a5da3cfa35e686a265c9

* O Arquivo não precisa ter o mesmo nome do comando flash que utilizaremos abaixo. Se o arquivo estiver comprimido em zip ou tar, faça a descompactação e utilize ele no comando de flash, heimdall não se importa com o nome da imagem basta que você utilize a partição correta

* Deslique o seu Galaxy Tab 2 7.0 (GSM) e conecte o adaptador USB no computador, mas não no Galaxy Tab 2 7.0 (GSM), ainda.

* Faça o Boot no seu Galaxy Tab 2 7.0 (GSM) no modo de download. Basta precionar a tecla para abaixar o volume em conjunto com a tecla de ligar. Aceite o aviso que aparece no aparelho. Agora sim, conecte o cabo USB no aparelho
** Neste momento, se familiarize com os comandos do Flashing Heimdall abaixo, assim você estará preparado para qualquer acontecimento não usual
* No seu Mac, abra um terminal, no diretório onde a recovery image está digite:
* heimdall flash --RECOVERY recovery.img --no-reboot

* Uma barra de transferência azul irá aparecer no dipositivo mostrando que a imagem está sendo transferida.

* Agora você pode fazer o reboot manual do aparelho no modo CloworkMod Recovery, basta pressionar o botão de ligar em conjunto com botão de aumentar o volume.

* Faça o download da versão do Cyanogenmod que você gostaria de instalar. <a href="http://download.cyanogenmod.org/?device=p3100">Aqui estão os downloads para este aparelho (Samsung galaxy tab 2 7.0 (gsm))</a>. 

* Coloque este arquivo em um cartão micro-sd e insira o cartão no aparelho

* Com o reboot feito, precisaremos formatar algumas pastas do aparelho para a nova versão funcionar corretamente.

* entre no menu "mounts and storage", iremos formatar as seguintes pastas (chamamos esta ação de full wipe):
* /system
* /cache
* /data
* depois disso, iremos no menu "advanced" e após no menu "dalvik cache", escolha a opção de "Wipe Dalvik Cache"

* Agora com o nosso sistema limpo, iremos efetuar a isntalação da Versão do Cyanogenmod que baixamos (eu aconselho baixar uma versão stable, para evitar alguns problemas)

* No menu iremos escolher a opção, install zip from sdcard
* Agora escolha a opção "choose zip from external sdcard"
* Escolha o ZIP da versão do Cyanogenmod que você baixou e isntale.

* Pronto, basta efetuar o reboot no aparelho e a nova versão estará instalada. No menu raiz existe a opção "reboot system now"



