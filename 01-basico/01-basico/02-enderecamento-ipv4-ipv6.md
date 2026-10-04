# Endereçamento de IPv4 e IPv6

## Endereçamento de IP

Todo dispositivo em uma rede precisa de um endereço único para ser identificado — assim como um endereço residencial identifica uma casa. Esse é o **endereço IP**.

- **IPv4**: formato `x.x.x.x`, com cada `x` variando de 0 a 255 (ex: `192.168.1.10`). Possui cerca de 4,3 bilhões de endereços possíveis, número que já se esgotou frente ao crescimento da internet.
- **IPv6**: criado para resolver o esgotamento do IPv4, usa endereços de 128 bits, representados em hexadecimal (ex: `2001:0db8:85a3:0000:0000:8a2e:0370:7334`), com uma quantidade de endereços praticamente inesgotável.

Existem também os **IPs privados** (usados dentro de redes locais, como `192.168.x.x`, `10.x.x.x`) e **IPs públicos** (usados para identificar a rede na internet).

## CIDR e Máscara de rede

A **máscara de rede** define qual parte do endereço IP identifica a rede e qual parte identifica o dispositivo (host) dentro dela.

- Exemplo: `255.255.255.0` significa que os 3 primeiros octetos identificam a rede, e o último identifica o host.

O **CIDR** (Classless Inter-Domain Routing) é uma forma simplificada de representar a máscara, usando uma barra seguida de um número, que indica quantos bits são usados para a rede:

- `/24` = `255.255.255.0` → 256 endereços possíveis (254 utilizáveis)
- `/16` = `255.255.0.0` → 65.536 endereços possíveis
- `/8` = `255.0.0.0` → mais de 16 milhões de endereços possíveis

Quanto menor o número depois da barra, maior a rede (mais hosts possíveis).

## DHCP - Dynamic Host Configuration Protocol

O DHCP é o protocolo responsável por **atribuir automaticamente** endereços IP (e outras configurações de rede, como gateway e DNS) aos dispositivos que entram na rede, sem precisar configurar manualmente cada um.

Funcionamento básico (processo conhecido como **DORA**):
1. **Discover** — o dispositivo entra na rede e pergunta "tem algum servidor DHCP aqui?"
2. **Offer** — o servidor DHCP responde oferecendo um endereço IP disponível
3. **Request** — o dispositivo solicita formalmente aquele endereço
4. **Acknowledge** — o servidor confirma e o dispositivo passa a usar aquele IP

Sem DHCP, cada dispositivo precisaria ter o IP configurado manualmente (IP fixo/estático), o que é inviável em redes grandes.
