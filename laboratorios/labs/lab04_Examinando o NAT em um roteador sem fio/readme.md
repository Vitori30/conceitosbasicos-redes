# Lab 04 - Examinando o NAT em um Roteador Wireless

## 🎯 Objetivo
Examinar o funcionamento do NAT (Network Address Translation) em um roteador wireless, configurar clientes utilizando DHCP e analisar a tradução de endereços durante a comunicação entre a rede local e a Internet.

## 📂 Componentes
- 1 Roteador Wireless
- 4 PCs
- Servidor Web (ciscolearn.nat.com)
- Cabos Ethernet (Copper Straight-Through)
- Cisco Packet Tracer

## ⚙️ Configuração
- Conexão dos quatro computadores ao roteador wireless.
- Configuração dos clientes para obter endereço IP automaticamente via DHCP.
- Acesso à interface de gerenciamento do roteador.
- Verificação da configuração da rede local e da conexão com a Internet.
- Análise do endereço IP da interface WAN e da rede LAN.

## 🧪 Testes
- Obter endereço IP automaticamente utilizando DHCP.
- Verificar a configuração da rede com o comando `ipconfig /all`.
- Confirmar os endereços IP atribuídos aos clientes.
- Criar uma PDU Complexa utilizando o protocolo HTTP.
- Observar o tráfego no modo **Simulation**.
- Analisar a tradução NAT comparando os cabeçalhos de entrada (Inbound) e saída (Outbound).

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
- Monitoramento do tráfego utilizando o modo Simulation.

## ✅ Resultado Esperado
Os computadores recebem automaticamente endereços IP privados via DHCP, comunicam-se com a rede externa através do roteador wireless e a tradução NAT é realizada corretamente, permitindo o acesso ao servidor Web.
