# Lab 04 - Examinando o NAT em um Roteador Wireless

## 🎯 Objetivo
Neste laboratório analisei como o NAT funciona no roteador Wi-Fi, configurei os clientes via DHCP e observei como os endereços foram traduzidos quando a rede local se comunicou com a Internet.

## 📂 Componentes
- 1 Roteador Wireless  
- 4 PCs  
- Servidor Web (**ciscolearn.nat.com**)  
- Cabos Ethernet (Copper Straight-Through)  
- Cisco Packet Tracer  

## ⚙️ Configuração
- Conectei os PCs ao roteador wireless  
- Configurei os clientes para obter endereço IP automaticamente via DHCP  
- Acessei a interface de gerenciamento do roteador  
- Verifiquei a configuração da rede local e a conexão com a Internet  
- Analisei o endereço IP da interface WAN e da rede LAN  

## 🧪 Testes
- Obtive endereço IP automaticamente utilizando DHCP  
- Verifiquei a configuração da rede com o comando:
  ```bash
  ipconfig /all

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

## ✅ Verificação Final
Os PCs receberam IP privado via DHCP, conseguiram acessar a Internet pelo roteador e o NAT traduziu os endereços corretamente, permitindo que a rede local se comunicasse com o servidor Web.

