# Módulo 2 - Ping na Prática

## Ping no Windows

No Windows, o ping é executado via Prompt de Comando (CMD) ou PowerShell:

```
ping 8.8.8.8
ping google.com
```

Por padrão, o Windows envia 4 pacotes e exibe o tempo de resposta de cada um, além de um resumo com pacotes enviados, recebidos, perdidos e o tempo mínimo/máximo/médio de resposta.

Parâmetros úteis:
- `ping -t endereco` → envia pings continuamente até ser interrompido manualmente (Ctrl+C)
- `ping -n 10 endereco` → define quantos pacotes enviar (nesse caso, 10)

## Ping no celular

Em smartphones (Android/iOS), o ping geralmente não vem como app nativo, mas pode ser usado através de:
- Aplicativos específicos de rede disponíveis nas lojas de aplicativos
- Apps de terminal (que simulam um ambiente de linha de comando)

O funcionamento é o mesmo: o app envia requisições ICMP para o endereço informado e exibe o tempo de resposta, sendo útil para testar a conectividade da rede Wi-Fi ou dados móveis diretamente do celular, sem precisar de um computador por perto.
