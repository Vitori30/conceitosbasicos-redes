# Lab 07 - A Interação do Cliente

## 🎯 Objetivo
Neste laboratório, observei como ocorre a interação entre um cliente e um servidor, acompanhando o processo de resolução de nomes (DNS) e o carregamento de uma página Web por meio do protocolo HTTP.

## 📂 Componentes
- 1 PC
- 1 Servidor
- Cisco Packet Tracer

## ⚙️ Configuração
- Acessei o modo **Simulation**.
- Configurei os filtros para visualizar apenas os protocolos **DNS** e **HTTP**.
- Utilizei o navegador Web do PC para acessar o endereço `www.example.com`.
- Executei a simulação para acompanhar a comunicação entre o cliente e o servidor.
- Analisei as informações das PDUs em cada etapa da comunicação.

## 🧪 Testes
- Configurei os filtros para capturar apenas eventos DNS e HTTP.
- Solicitei a página Web utilizando o navegador do PC.
- Observei a resolução do nome de domínio pelo servidor DNS.
- Acompanhei a solicitação e o envio da página Web pelo servidor HTTP.
- Analisei as informações das PDUs utilizando a janela **PDU Information**.
- Percorri as camadas do modelo OSI para compreender o fluxo da comunicação.

## 🛠️ Tecnologias utilizadas
- Cisco Packet Tracer
- DNS (Domain Name System)
- HTTP (HyperText Transfer Protocol)
- Modelo OSI
- Simulation Mode

## 💡 Habilidades desenvolvidas
- Compreensão da comunicação entre cliente e servidor.
- Análise da resolução de nomes utilizando o protocolo DNS.
- Identificação do funcionamento do protocolo HTTP.
- Interpretação das PDUs durante a comunicação em rede.
- Análise do tráfego utilizando o modo **Simulation**.
- Compreensão do fluxo da comunicação entre as camadas do modelo OSI.

## ✅ Verificação Final
Verifiquei que o cliente solicita ao servidor DNS a resolução do nome de domínio para um endereço IP. Após essa etapa, o cliente estabelece comunicação com o servidor HTTP, que responde enviando a página Web solicitada, permitindo visualizar todo o processo de comunicação no modo **Simulation**.
