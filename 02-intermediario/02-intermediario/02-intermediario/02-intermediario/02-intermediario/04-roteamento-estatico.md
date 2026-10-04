# Módulo 04: Roteamento Estático

## Aula 01 - Introdução ao Roteamento IP Estático

Roteamento estático é quando as rotas (caminhos entre redes) são configuradas **manualmente** pelo administrador da rede, em vez de serem aprendidas automaticamente. É indicado para redes pequenas ou com topologia simples e estável, onde o controle manual é mais simples que configurar um protocolo de roteamento dinâmico.

## Aula 02 - Laboratório Roteamento Estático

Na prática, uma rota estática é configurada informando: a rede de destino, a máscara dessa rede, e o próximo salto (next-hop) — ou seja, o IP do roteador por onde aquele tráfego deve passar para chegar ao destino. Cada roteador da rede precisa ter as rotas estáticas necessárias para alcançar todas as redes que não estão diretamente conectadas a ele.

## Aula 03 - Adicionando novos Roteadores

Ao expandir a rede com novos roteadores, é necessário atualizar as tabelas de rotas estáticas em todos os equipamentos envolvidos, garantindo que cada um saiba como alcançar as novas redes adicionadas. Esse processo pode se tornar trabalhoso em redes maiores, sendo um dos motivos pelos quais protocolos de roteamento dinâmico (como OSPF ou BGP) são usados em ambientes mais complexos.
