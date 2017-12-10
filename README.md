Automação Residencial
===================================================

Basicamente o projeto de automação foi divido em duas etapas:
```
1) Definição dos Hardwares
2) Definição do Software de Controle
```

<h3> Definições </h3>

Durante os estudos de para o projeto de automação residencial foi visto que havia vários hardware o primeiro dele foi o Arduino https://www.arduino.cc/en/Main/Products. Esse se demonstrou muito eficiente mas a parte de interação gráfica levaria a um desenvolvimento muito longo e não seria algo que daria para aproveitar para outros usuários, mesmo disponibilizando o código fonte.

Passando para outros testes foi encontrado dispostivios da Broadlink http://www.ibroadlink.com/sp3/ e os demais modelos. Essas tomadas seriam de grande utilizade para poder fazer automações e criação de cenas mas isso dependeria do aplicativo próprio da tomada o que não permitia a integração/automação entre outros hardwares.

Após buscas na internet encontrei um o Sonoff https://www.itead.cc/sonoff-wifi-wireless-switch.html o que tive a impressão que seria meu hardware principal pelo baixo custo. Mas apresentava o mesmo problema dos demais hardwares que foi encontrado no mercado: se tivesse três hardwares de diferentes fabricantes seria necessários três aplicativos o que tornaria inviável o projeto de automação residencial.

Então depois de um tempo buscando algo interessantes na Internet encontrei um vídeo o youtube https://www.youtube.com/watch?v=diTQ3M5zH-0 que resolveria todos os meus problemas:

Conheci o Home Assistant: https://home-assistant.io/

Depois de um tempo lendo a sobre o Home Assistant deu pra perceber que a plataforma era excelente que além de 'resolver meus problemas' com od dispositivos era Open Source(que maravilha!!! :)), baseando na Web e desenvolvido em Python. Deu pra perceber que o Home Assistant trabalha com componentes que nada mais é do que plataforma para dispostivos ou serviços que são possíveis a integração entre eles o que se torna muito flexível o processo de integração e automação.

Bem, depois de ter encontrado o Home Assistant a próxima definição seria: Onde rodar este sistema?

Como já tinha um experiência de algum tempo com o Raspberry Pi(desde a versão 1) https://www.raspberrypi.org/products/ e já tinha aproximadamente 3 unidadas em casa optei usá-lo, a versão utilizada foi igual a esta https://produto.mercadolivre.com.br/MLB-697674443-raspberry-pi-modelo-b-plus-512mb-4-usb-arm1176jzf-s-700mhz-_JM. Além de ter em casa o preço é bem em conta pelo potencial que e ele e a entrega que ele proporciona.

<h3> Passos com o Raspberry PI </h3>

Existem vários sistemas operacionais para o Raspberry e disponível para download https://www.raspberrypi.org/downloads/ mas resolvi instar o Raspbian que, conforme informei antes, já tinha tido mais contato anteriormente.

Depois de instalado o Raspbian dava início a instalação do Home Assistant.
A instalação do Home Assistant é bem complicada tem que seguir os passos corretamente.

Para instalação pelo site oficial do HA só seguir o link https://home-assistant.io/getting-started/.

No meu caso eu segui os passos do link do youtube https://www.youtube.com/watch?v=GjzOXkPb7XE&t=329s, com os seguintes passos:

logado no raspberry, abra o terminal e execute os comandos:
* sudo raspi-config
* sudo apt-get update
* sudo apt-get upgrade
* sudo reboot
* sudo pip3 install homeassistant
* sudo nano /etc/init.d/hass-daemon, copy the script, change user to root
* sudo chmod +x /etc/init.d/hass-daemon
* sudo update-rc.d hass-daemon defaults
* sudo service hass-daemon install
* sudo reboot

Com isso, no meu caso, o sistema subiu e funcionou normalmente.

<h3> Configurações do Home Assistant </h3>

Após a instalação do sistemas chegou a hora de configurar os componentes/serviços:

O Home Assistant possui componente específicos para sua plataforma e alguns configurados são:

<ul> <b>config: </b> https://home-assistant.io/components/config/
