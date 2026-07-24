# Lab 03 - Configuração do DHCP em um Roteador Wireless

## 🎯 Objetivo
Neste laboratório configurei o DHCP no roteador Wi-Fi, defini uma nova faixa de IPs e os PCs receberam automaticamente as configurações de rede, conectando-se à rede local e acessando a Internet sem erros.

## 📂 Componentes
- 1 Roteador Wireless
- 3 PCs (PC0, PC1 e PC2)
- Cabos Ethernet (Copper Straight-Through)
- Cisco Packet Tracer

## ⚙️ Configuração
- Conectei os três PCs ao roteador wireless  
- Alterei o endereço IP do roteador para **192.168.5.1**  
- Habilitei o DHCP  
- Configurei o endereço inicial da faixa DHCP como **192.168.5.126**  
- Defini o número máximo de usuários como **75**  
- Configurei os PCs para obter IP automático via DHCP  

## 🧪 Testes
- Renovei o endereço IP utilizando DHCP  
- Verifiquei a configuração com o comando:
  ```bash
  ipconfig

## 🛠️ Tecnologias utilizadas
- Cisco Packet Tracer
- DHCP
- IPv4
- Ethernet
- Roteador Wireless
- Command Prompt (ipconfig e ping)

## 💡 Habilidades desenvolvidas
- Configuração de DHCP em roteador wireless.
- Alteração da faixa de endereços IP da rede.
- Configuração automática de clientes utilizando DHCP.
- Renovação de endereço IP.
- Verificação da configuração de rede com **ipconfig**.
- Testes de conectividade utilizando **ping**.

## ✅ Verificação Final
Todos os computadores receberam IP da nova faixa, conseguem comunicaram com o roteador e entre si, confirmando que o DHCP tá funcionando corretamente.
