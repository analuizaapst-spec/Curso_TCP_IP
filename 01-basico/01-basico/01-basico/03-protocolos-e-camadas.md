# Principais protocolos e suas camadas

## Aplicação (Camada 7)

É a camada mais próxima do usuário, onde os programas interagem diretamente com a rede. Exemplos de protocolos: **HTTP/HTTPS** (navegação web), **FTP** (transferência de arquivos), **SMTP/IMAP** (e-mail), **DNS** (tradução de nomes em IPs).

## Apresentação (Camada 6)

Responsável por traduzir, criptografar e compactar os dados, garantindo que o formato enviado por um sistema seja entendido pelo outro, independente da plataforma. Exemplos: criptografia SSL/TLS, formatos como JPEG, codificação de caracteres.

## Sessão (Camada 5)

Gerencia a abertura, manutenção e encerramento das "sessões" de comunicação entre dois dispositivos, controlando quando a conexão deve ser iniciada, pausada ou finalizada.

## Transporte (Camada 4)

Garante que os dados cheguem corretamente ao destino, controlando ordem, integridade e, em alguns casos, confirmação de entrega. Os dois principais protocolos dessa camada:

- **TCP** (Transmission Control Protocol): orientado à conexão, confiável, garante entrega e ordem dos pacotes (usado em navegação web, e-mail).
- **UDP** (User Datagram Protocol): mais rápido, mas sem garantia de entrega (usado em streaming, jogos online, chamadas de voz/vídeo).

## Rede (Camada 3)

Responsável pelo **endereçamento lógico** (IP) e pelo **roteamento** dos pacotes entre redes diferentes. É aqui que entram os roteadores e o protocolo **IP** (IPv4/IPv6).

## Enlace (Camada 2)

Controla a comunicação entre dispositivos na **mesma rede local**, usando endereços físicos (**MAC Address**). É a camada onde atuam os **switches**.

## Física (Camada 1)

É a camada responsável pela transmissão real dos bits através do meio físico: cabos de rede, fibra óptica, sinais de rádio (Wi-Fi), conectores, etc.

## Conceitos intermediários que você precisa aprender no básico

Para avançar no estudo de redes, é importante já sair do básico com uma base sólida nos seguintes pontos:
- Diferença entre domínio de colisão e domínio de broadcast
- Como funciona a comunicação entre redes diferentes (necessidade de um roteador/gateway)
- Noção inicial de portas lógicas (ex: porta 80 para HTTP, porta 443 para HTTPS)
- Diferença entre switch (camada 2) e roteador (camada 3)
