# Lab 12 - Usando o Comando `ping`

## 🎯 Objetivo
Neste laboratório, utilizei o comando `ping` para identificar problemas de conectividade em uma rede, analisando a comunicação entre os computadores e um servidor Web e corrigindo configurações incorretas.

## 📂 Componentes
- PCs da rede
- Servidor Web (`www.cisco.pka`)
- Servidor DNS
- Cisco Packet Tracer

## ⚙️ Configuração
- Testei o acesso ao servidor Web utilizando o navegador.
- Identifiquei os computadores que apresentavam falha de conexão.
- Executei o comando `ping` utilizando o nome de domínio e o endereço IP do servidor.
- Comparei as configurações de rede utilizando o comando `ipconfig /all`.
- Corrigi a configuração do servidor DNS nos computadores com problema.
- Verifiquei novamente a conectividade após a correção.

## 🧪 Testes
- Acessei `www.cisco.pka` pelo navegador Web.
- Executei `ping www.cisco.pka`.
- Executei `ping` utilizando o endereço IP do servidor Web.
- Comparei as configurações de DNS utilizando `ipconfig /all`.
- Corrigi as configurações em **IP Configuration**.
- Confirmei o acesso ao servidor Web após a correção.

## 🛠️ Tecnologias utilizadas
- Cisco Packet Tracer
- ICMP (Ping)
- DNS (Domain Name System)
- IPv4
- Command Prompt
- Navegador Web

## 💡 Habilidades desenvolvidas
- Diagnóstico de problemas de conectividade.
- Utilização do comando `ping`.
- Verificação da resolução de nomes pelo servidor DNS.
- Comparação de configurações de rede.
- Correção de configurações incorretas de DNS.
- Validação da comunicação entre cliente e servidor.

## ✅ Verificação Final
Verifiquei que um computador pode conseguir alcançar o servidor pelo endereço IP, mas não pelo nome de domínio quando existe uma configuração incorreta do servidor DNS. Após corrigir essa configuração, a comunicação com o servidor Web foi restabelecida.
