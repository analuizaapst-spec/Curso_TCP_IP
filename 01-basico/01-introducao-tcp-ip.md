# Introdução ao TCP/IP

## Por que estudar Redes IP

O protocolo TCP/IP é a base de praticamente toda comunicação de dados hoje, incluindo a internet. Entender como ele funciona é essencial para configurar redes, diagnosticar problemas de conectividade, trabalhar com servidores, segurança da informação e suporte técnico. Sem esse conhecimento, fica difícil entender por que um dispositivo "não conecta", por que um site não carrega, ou como dois computadores conseguem trocar informações mesmo estando em redes diferentes.

## Sistema Binário, onde tudo começa...

Computadores processam informação usando apenas dois estados: 0 e 1 (ligado/desligado). Esse é o sistema binário, base de tudo na computação, incluindo os endereços IP.

- Cada posição binária é chamada de **bit**.
- Um conjunto de 8 bits forma um **byte** (ou octeto).
- Endereços IPv4 são formados por **4 octetos** (32 bits no total), por isso vemos algo como `192.168.0.1` — cada número representa um octeto convertido de binário para decimal.

Exemplo: o octeto `11000000` em binário equivale a `192` em decimal.

## Modelo OSI de Referência

O Modelo OSI (Open Systems Interconnection) é um modelo teórico criado para padronizar como os sistemas de rede se comunicam, dividindo o processo em **7 camadas**, cada uma com uma responsabilidade específica:

1. Física
2. Enlace
3. Rede
4. Transporte
5. Sessão
6. Apresentação
7. Aplicação

Cada camada só se comunica diretamente com a camada acima e abaixo dela, o que facilita a organização, o diagnóstico de problemas e a criação de novas tecnologias sem quebrar o resto do sistema.

## Camadas TCP/IP

O modelo TCP/IP é uma versão mais prática (usada de fato na internet), com **4 camadas**, que resume as 7 camadas do OSI:

| Camada TCP/IP | Equivalente no OSI |
|---|---|
| Aplicação | Aplicação, Apresentação, Sessão |
| Transporte | Transporte |
| Internet | Rede |
| Acesso à Rede | Enlace, Física |

É esse modelo que rege o funcionamento real da internet e das redes locais no dia a dia.
