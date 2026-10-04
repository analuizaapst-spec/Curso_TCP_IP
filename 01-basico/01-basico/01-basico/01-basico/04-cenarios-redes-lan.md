# Cenários de Redes LAN

## Topologias

Topologia é a forma como os dispositivos de uma rede estão fisicamente ou logicamente conectados entre si. As mais comuns:

- **Barramento**: todos os dispositivos conectados a um único cabo central (pouco usada hoje).
- **Estrela**: todos os dispositivos conectados a um ponto central (switch/roteador) — é o padrão mais usado atualmente em redes LAN.
- **Anel**: cada dispositivo se conecta a dois outros, formando um círculo.
- **Malha (mesh)**: cada dispositivo se conecta a vários outros, aumentando redundância e tolerância a falhas.

## Hardwares de redes

- **Switch**: conecta dispositivos dentro da mesma rede local, encaminhando dados com base no endereço MAC (camada 2).
- **Roteador**: conecta redes diferentes entre si (ex: sua rede local à internet), encaminhando pacotes com base no endereço IP (camada 3).
- **Access Point (AP)**: fornece acesso à rede via Wi-Fi.
- **Modem**: converte o sinal da operadora (fibra, cabo, etc.) em um sinal que o roteador consegue usar.

## Rede simples com Roteador

O cenário mais básico de uma rede doméstica ou pequeno escritório: um roteador central distribuindo internet (via cabo ou Wi-Fi) para os dispositivos conectados, geralmente com DHCP ativo atribuindo IPs automaticamente a cada um.

## Rede com Roteador e Dispositivos Gerenciáveis

Em redes um pouco mais estruturadas, usam-se switches **gerenciáveis**, que permitem configurações avançadas como VLANs, controle de tráfego, monitoramento de portas e maior segurança, diferente de um switch simples ("burro"), que apenas encaminha pacotes sem nenhuma inteligência extra.

## Rede com VLAN's

**VLAN** (Virtual Local Area Network) permite dividir uma rede física em várias redes lógicas separadas, mesmo usando o mesmo switch físico. Isso é usado para:
- Separar tráfego por setor (ex: VLAN para TI, VLAN para financeiro)
- Aumentar a segurança, isolando o tráfego entre grupos
- Reduzir o domínio de broadcast, melhorando performance

Cada VLAN se comporta como se fosse uma rede física independente, mesmo compartilhando a mesma infraestrutura.
