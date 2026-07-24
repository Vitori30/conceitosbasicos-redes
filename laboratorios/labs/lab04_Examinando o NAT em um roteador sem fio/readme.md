# Lab 04 - Examinando o NAT em um Roteador Wireless

## 🎯 Objetivo
Entender como o NAT funciona no roteador Wi-Fi, configurar os clientes via DHCP e analisar como os endereços são traduzidos quando a rede local comunica com a Internet.

## 📂 Componentes
- 1 Roteador Wireless
- 4 PCs
- Servidor Web (ciscolearn.nat.com)
- Cabos Ethernet (Copper Straight-Through)
- Cisco Packet Tracer

## ⚙️ Configuração
- PCs conectados ao roteador wireless.
- Clientes obtendo endereço IP automaticamente via DHCP.
- Acesso à interface de gerenciamento do roteador.
- Verificação da configuração da rede local e da conexão com a Internet.
- Análise do endereço IP da interface WAN e da rede LAN.

## 🧪 Testes
- Obter endereço IP automaticamente utilizando DHCP.
- Verificar a configuração da rede com o comando `ipconfig /all`.
- Vaidar IP atribuídos aos clientes.
- Criar uma PDU Complexa utilizando o protocolo HTTP.
- Observar o tráfego no modo **Simulation**.
- Comparar a tradução NAT comparando os cabeçalhos de entrada (Inbound) e saída (Outbound).

## 🛠️ Tecnologias utilizadas
- Cisco Packet Tracer
- NAT (Network Address Translation)
- DHCP
- IPv4
- HTTP
- Simulation Mode
- Command Prompt (`ipconfig /all`)

## 💡 Habilidades desenvolvidas
- Configuração de clientes utilizando DHCP.
- Identificação de endereços IP públicos e privados.
- Compreensão do funcionamento do NAT.
- Análise da tradução de endereços IP.
- Interpretação dos cabeçalhos de pacotes.
- Monitorar tráfego utilizando o modo Simulation.

## ✅ Resultado Esperado
Os PCs recebem IP privado via DHCP, conseguem acessar a Internet pelo roteador e o NAT traduz os endereços corretamente, permitindo que a rede local se comunique com o servidor Web.
