# Lab 08 - Observando Solicitações Web

## 🎯 Objetivo
Neste laboratório, visualizei o tráfego entre um cliente e um servidor Web, analisando como ocorre a comunicação durante uma solicitação HTTP e observando o funcionamento do protocolo por meio do modo **Simulation**.

## 📂 Componentes
- 1 External Client
- 1 Servidor Web (ciscolearn.web.com)
- Servidor DNS
- Cisco Packet Tracer

## ⚙️ Configuração
- Verifiquei a conectividade com o servidor utilizando o comando `ping`.
- Acessei o servidor Web pelo navegador utilizando a URL `ciscolearn.web.com`.
- Analisei o código HTML da página hospedada no servidor.
- Configurei os filtros do modo **Simulation** para visualizar apenas os protocolos TCP e HTTP.
- Criei uma PDU Complexa para acompanhar o tráfego entre o cliente e o servidor.

## 🧪 Testes
- Executei o comando `ping ciscolearn.web.com`.
- Verifiquei a resolução do nome de domínio para um endereço IP.
- Acessei a página Web utilizando o navegador.
- Comparei o código HTML do servidor com a página exibida no navegador.
- Executei a simulação da comunicação HTTP.
- Observei o fluxo dos pacotes e o estabelecimento da conexão TCP.
- Analisei os eventos registrados no **Simulation Panel**.

## 🛠️ Tecnologias utilizadas
- Cisco Packet Tracer
- DNS (Domain Name System)
- HTTP (HyperText Transfer Protocol)
- TCP (Transmission Control Protocol)
- HTML
- Simulation Mode

## 💡 Habilidades desenvolvidas
- Verificação da conectividade utilizando o comando `ping`.
- Compreensão da resolução de nomes pelo servidor DNS.
- Análise da comunicação entre cliente e servidor Web.
- Interpretação do funcionamento do protocolo HTTP.
- Identificação do processo de estabelecimento da conexão TCP.
- Observação do fluxo de pacotes utilizando o modo **Simulation**.

## ✅ Verificação Final
Verifiquei que o cliente utiliza o servidor DNS para resolver o nome do domínio em um endereço IP antes de estabelecer a conexão com o servidor Web. Também observei que o protocolo HTTP utiliza o TCP para garantir uma comunicação confiável entre cliente e servidor, permitindo o carregamento correto da página Web.
