<h3> Definições </h3>

<p> Componente: https://home-assistant.io/components/automation/  </p> 
<p> Configuração: https://github.com/dedynobre/homeassistant/blob/master/configuration.yaml </p>

<h4>Ar Condicionado (ar_condicionado.yaml) </h4>
  <ul> Desliga ar condicionado todos os dias entre as 23h e 06h quando a temperatura estiver abaixo de 24°C </ul>
  <ul> Liga ar condicionado todos os dias entre 23h e 06h quando a temperatura estiver acima de de 26°C</ul>
  <ul> Liga ar condicionado quando acionado <a href="https://pt.aliexpress.com/item/Original-Xiaomi-Mijia-Wireless-Switch-House-Control-Center-Intelligent-Multifunction-Smart-Home-Device-work-with-mi/32814699040.html?spm=a2g03.search0104.3.1.l1CTjn&ws_ab_test=searchweb0_0,searchweb201602_3_10152_10065_10151_10344_10068_5000016_10345_10342_10547_10343_51102_10340_5060016_10341_10548_5130016_10541_10084_10083_10307_10539_10312_10059_10313_5080016_10314_10534_100031_10604_10603_10103_10605_10594_10596_10142_10107,searchweb201603_25,ppcSwitch_5&algo_expid=20163a6a-7509-4978-9774-120130290621-0&algo_pvid=20163a6a-7509-4978-9774-120130290621&rmStoreLevelAB=0">Interruptor Xiaomi</a> com clique duplo e ar condicionado desligado </ul>
  <ul> Desliga Ar Condicionado quando acionado o Interruptor Xiaomi com clique duplo e ar condicionado ligado </ul>
    
<h4>Controle Televisão (controle_tv.yaml) </h4>
  <ul> Controle Volume - Aumentar </ul>
  <ul> Controle Volume - Diminuir </ul>
  <ul> Liga TV Quando horário atual for igual ao selecionado nos Input Number </ul>
  <ul> Desliga TV Quando horário atual for igual ao selecionado nos Input Number </ul>
  <ul> Ao ligar Receptor desliga Chrome Cast </ul>
  <ul> Ao ligar ChromeCast desliga Receptor </ul>
  
<h4>Controles (controles.yaml) </h4>
  <ul> Checa Localização - Chegando em Casa - Liga Dispositivos </ul>
  <ul> Checa Localização - Saindo de Casa - Desliga Dispositivos </ul>
  
<h4>Iluminação (iluminação.yaml) </h4>
  <ul> No geral verifica se está durante o dia(dependendo da posição do sol) e controla a iluminação do apartamento, ou seja, caso a luz esteja ligada durante o dia a lâmpada é desligada depois de um tempo definido na tela de iluminação. </ul>
  <ul> A ideia da automação é tentar garantir que não fique lâmpadas ligadas pela casa sem necessidade. </ul>
  
<h4>Controle Via Telegram (telegram_acionamentos.yaml) </h4>  
  <ul> Controle do apartamento via Aplicativo Telegram, via Chatbot. São feitos diversos acionamentos via Telegram, como ligar lampadas, controle de temperatura, checa temperatura dos cômodos. </ul>

