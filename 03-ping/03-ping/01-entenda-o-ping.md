# Módulo 1 - Entenda o Ping
 
## Por que estudar o ping?
 
O **ping** é uma das ferramentas mais simples e poderosas para diagnóstico de rede. Com um único comando, é possível verificar se um dispositivo está acessível na rede, medir o tempo de resposta (latência) e identificar perda de pacotes — informações essenciais para resolver problemas de conectividade no dia a dia, seja em suporte técnico, administração de redes ou uso pessoal.
 
## Princípios de funcionamento
 
O ping funciona enviando pacotes **ICMP Echo Request** para um endereço IP ou nome de domínio, e aguardando a resposta **ICMP Echo Reply** do destino.
 
- Se a resposta chega, o dispositivo está acessível, e o ping informa o tempo que a resposta levou (em milissegundos).
- Se não chega, pode indicar que o dispositivo está desligado, a rede está com problema, ou que um firewall está bloqueando o tráfego ICMP.
O protocolo ICMP opera na camada de Rede (camada 3), junto com o IP, sendo usado especificamente para mensagens de controle e diagnóstico, não para transporte de dados como o TCP ou UDP.
