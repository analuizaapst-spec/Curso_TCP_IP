# Módulo 03: Laboratório de Protocolos de Redes

## Aula 01 - STP - Introdução ao Spanning Tree Protocol

O **STP** é um protocolo usado para evitar **loops de rede** em topologias com links redundantes entre switches. Loops de rede causam broadcast storms, que podem derrubar a rede inteira. O STP identifica caminhos redundantes e bloqueia logicamente as portas que causariam loop, mantendo-as como backup caso o caminho principal falhe.

## Aula 02 - DHCP

Na prática, o DHCP pode ser configurado diretamente em um roteador ou em um servidor dedicado, definindo: faixa de IPs a ser distribuída, tempo de concessão (lease time), gateway padrão e servidores DNS que serão repassados automaticamente aos dispositivos da rede.

## Aula 03 - Link Aggregation

Também conhecido como **LACP** (Link Aggregation Control Protocol) ou "bonding", permite combinar **múltiplas conexões físicas** entre dois equipamentos em um único link lógico, aumentando a banda disponível e fornecendo redundância — se um dos cabos falhar, o tráfego continua pelos demais.

## Aula 04 - SNMP

O **SNMP** (Simple Network Management Protocol) é usado para **monitorar e gerenciar** dispositivos de rede remotamente (switches, roteadores, servidores), coletando informações como uso de CPU, tráfego de rede, status das portas, entre outros, geralmente através de um software de monitoramento central.
