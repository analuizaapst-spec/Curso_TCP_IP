# Módulo 02: Arquitetura de Rede

## Aula 01 - Lab Comandos iniciais

Primeiros comandos usados para acessar e configurar equipamentos de rede via linha de comando (CLI), geralmente através de interfaces de terminal como o console do switch/roteador, incluindo comandos básicos de navegação entre modos (modo usuário, modo privilegiado, modo de configuração).

## Aula 02 - Como funciona um Switch?

O switch opera na camada 2 (Enlace) e é responsável por conectar dispositivos dentro da mesma rede local. Ele aprende os endereços MAC dos dispositivos conectados a cada porta e monta uma **tabela MAC**, usada para encaminhar o tráfego diretamente para a porta correta, em vez de transmitir para todas as portas (o que reduz colisões e melhora a performance da rede).

## Aula 03 - Como funciona uma VLAN?

Na prática, configurar uma VLAN em um switch gerenciável envolve criar a VLAN (com um número de identificação, a VLAN ID) e associar as portas desejadas a ela. Dispositivos em VLANs diferentes não se enxergam diretamente — só se comunicam através de um roteador ou de um switch com capacidade de roteamento entre VLANs (**inter-VLAN routing**).

## Aula 04 - Como funciona um Roteador?

O roteador opera na camada 3 (Rede) e é responsável por conectar redes diferentes, decidindo o melhor caminho para encaminhar os pacotes com base no endereço IP de destino. Ele utiliza uma **tabela de roteamento**, que pode ser configurada manualmente (roteamento estático) ou aprendida automaticamente através de protocolos de roteamento dinâmico.
