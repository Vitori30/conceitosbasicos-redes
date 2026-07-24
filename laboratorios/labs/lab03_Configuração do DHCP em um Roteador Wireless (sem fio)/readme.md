# Lab 03 - Configuração do DHCP em um Roteador Wireless

## 🎯 Objetivo
Configurar o DHCP no roteador Wi-Fi, definindo uma nova faixa de IPs e deixar os PCs pegarem as configurações de rede automaticamente.

## 📂 Componentes
- 1 Roteador Wireless
- 3 PCs (PC0, PC1 e PC2)
- Cabos Ethernet (Copper Straight-Through)
- Cisco Packet Tracer

## ⚙️ Configuração
- Conexão dos três PCs ao roteador wireless.
- Endereço IP do roteador alterado para **192.168.5.1**.
- DHCP habilitado.
- Endereço inicial da faixa DHCP: **192.168.5.126**.
- Número máximo de usuários: **75**.
- PCs configurados pra pegar IP automático via DHCP.

## 🧪 Testes
- Renovação do endereço IP utilizando DHCP.
- Verificação da configuração com o comando:
  ```bash
  ipconfig
  ```
- Teste de conectividade com o roteador:
  ```bash
  ping 192.168.5.1
  ```
- Teste de conectividade entre os computadores:
  ```bash
  ping 192.168.5.126
  ping 192.168.5.127
  ```
- Confirmação de que todos os dispositivos responderam corretamente aos testes de comunicação.

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

## ✅ Resultado Esperado
Todos os computadores recebem IP da nova faixa, conseguem comunicar com o roteador e entre si, confirmando que o DHCP tá funcionando.
