# Módulo 3 - Cenários

## Metodologia de diagnóstico

Ao usar o ping para investigar um problema de rede, uma abordagem eficiente é testar "de dentro pra fora":
1. Ping no próprio gateway (roteador local) — confirma se o problema é local ou externo
2. Ping em um IP público conhecido (ex: `8.8.8.8`) — testa se há saída para a internet
3. Ping em um domínio (ex: `google.com`) — testa se o problema está relacionado à resolução de DNS

Esse processo ajuda a isolar rapidamente onde está o problema: no dispositivo, na rede local, no provedor de internet ou na resolução de nomes.

## Cliente que reclama toda hora

Em cenários de suporte, é comum lidar com clientes que relatam "a internet cai direto", mesmo sem um padrão claro. Nesses casos, o ping contínuo (`ping -t`) é uma ferramenta valiosa: deixar rodando por um período prolongado permite identificar se há **perda de pacotes intermitente** ou picos de latência que coincidem com os horários relatados pelo cliente, ajudando a confirmar (ou descartar) se o problema é realmente de rede.

## Cenário com roteadores inteligentes

Roteadores mais modernos ("inteligentes"), com recursos como QoS, mesh ou firmwares customizados, às vezes bloqueiam ou limitam respostas ICMP por padrão, como medida de segurança. Isso pode fazer parecer que um dispositivo está "fora do ar" quando na verdade só está ignorando o ping — por isso é importante, nesses cenários, confirmar a conectividade por outros meios (como acessar um serviço na porta específica) antes de concluir que há um problema real de rede.
