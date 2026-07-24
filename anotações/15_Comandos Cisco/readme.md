# 🧠 Comandos Cisco

## Mapa Mental

COMANDOS CISCO
│
├── O que são?
│   └── Instruções utilizadas para configurar e verificar equipamentos Cisco.
│
├── Interface de acesso
│   ├── Console
│   ├── SSH
│   └── Telnet
│
├── Modos de operação
│   ├── User EXEC
│   ├── Privileged EXEC
│   └── Global Configuration
│
├── Configuração básica
│   ├── Nome do equipamento
│   ├── Senhas
│   ├── IP das interfaces
│   └── Salvar configurações
│
├── Verificação
│   ├── Status das interfaces
│   ├── Tabela de roteamento
│   ├── Configurações
│   └── Conectividade
│
└── Principais comandos
    ├── show
    ├── configure terminal
    ├── interface
    ├── ip address
    ├── no shutdown
    ├── ping
    └── copy running-config startup-config

---

# O que são comandos Cisco?

Os **comandos Cisco** são instruções utilizadas para configurar, administrar e verificar equipamentos de rede, como:

- Roteadores.
- Switches.
- Firewalls.
- Access Points.

Eles são utilizados através da **CLI (Command Line Interface)**, uma interface de comandos onde o administrador controla o equipamento.

---

# Explicando de forma simples

Imagine um carro.

🚗 O painel mostra informações.

🔧 O mecânico utiliza comandos para configurar e verificar o funcionamento.

Nos equipamentos Cisco, a CLI funciona como esse painel de controle.

O administrador utiliza comandos para dizer ao equipamento o que deve ser feito.

---

# Modos de operação Cisco

Os equipamentos Cisco possuem diferentes níveis de acesso.

---

# 1️⃣ User EXEC Mode

Representado por:

```
Router>
```

É o modo inicial.

Permite comandos básicos de consulta.

Exemplo:

```
ping
```

---

# 2️⃣ Privileged EXEC Mode

Representado por:

```
Router#
```

Permite visualizar informações mais completas.

Para entrar:

```
enable
```

Exemplo:

```
Router> enable
Router#
```

---

# 3️⃣ Global Configuration Mode

Representado por:

```
Router(config)#
```

Usado para alterar configurações do equipamento.

Para entrar:

```
configure terminal
```

ou

```
conf t
```

---

# Comandos básicos de navegação

## Entrar no modo privilegiado

```
enable
```

---

## Entrar no modo de configuração

```
configure terminal
```

ou

```
conf t
```

---

## Sair de um modo

Voltar um nível:

```
exit
```

Sair completamente:

```
end
```

---

# Configuração básica do equipamento

## Alterar nome do equipamento

Comando:

```
hostname NOME
```

Exemplo:

```
hostname R1
```

Resultado:

```
R1(config)#
```

---

## Configurar senha de acesso privilegiado

```
enable secret senha
```

Exemplo:

```
enable secret cisco123
```

---

## Configurar senha do console

Entrar na linha console:

```
line console 0
```

Adicionar senha:

```
password senha
```

Ativar solicitação de senha:

```
login
```

---

# Configuração de endereço IP

Entrar na interface:

```
interface gigabitEthernet 0/0
```

Adicionar IP:

```
ip address endereço máscara
```

Exemplo:

```
ip address 192.168.1.1 255.255.255.0
```

Ativar a interface:

```
no shutdown
```

---

# Verificação de interfaces

## Mostrar interfaces

```
show interfaces
```

---

## Ver resumo das interfaces

```
show ip interface brief
```

Mostra:

- Interface.
- Endereço IP.
- Estado da porta.

Exemplo:

```
Gig0/0    192.168.1.1    up
```

---

# Comandos de teste

## Testar comunicação

```
ping endereço_IP
```

Exemplo:

```
ping 192.168.1.10
```

Verifica se existe comunicação entre dispositivos.

---

## Rastrear caminho

```
traceroute endereço_IP
```

Mostra o caminho percorrido pelos pacotes.

---

# Comandos de configuração e memória

## Ver configuração atual

```
show running-config
```

Mostra a configuração que está funcionando naquele momento.

---

## Ver configuração salva

```
show startup-config
```

Mostra a configuração armazenada na memória.

---

## Salvar configuração

```
copy running-config startup-config
```

ou:

```
write
```

Salva as alterações para não serem perdidas após reiniciar.

---

# Comandos de roteamento

## Ver tabela de roteamento

```
show ip route
```

Mostra os caminhos conhecidos pelo roteador.

---

## Adicionar rota estática

```
ip route rede máscara próximo_salto
```

Exemplo:

```
ip route 192.168.2.0 255.255.255.0 10.0.0.2
```

---

# Comandos de Switch

## Ver tabela MAC

```
show mac address-table
```

Mostra os dispositivos aprendidos pelo switch.

---

## Ver informações do switch

```
show version
```

Mostra:

- Modelo.
- Versão do IOS.
- Tempo ligado.

---

# Comandos importantes no Packet Tracer

## Ver dispositivos conectados

```
show cdp neighbors
```

---

## Ver detalhes das conexões

```
show cdp neighbors detail
```

---

# Principais comandos resumidos

| Comando | Função |
|---|---|
| enable | Entra no modo privilegiado |
| conf t | Entra na configuração global |
| hostname | Define nome do equipamento |
| interface | Acessa uma interface |
| ip address | Configura IP |
| no shutdown | Ativa interface |
| show running-config | Mostra configuração atual |
| show startup-config | Mostra configuração salva |
| show ip interface brief | Mostra resumo das interfaces |
| show ip route | Mostra tabela de roteamento |
| show mac address-table | Mostra tabela MAC |
| ping | Testa conexão |
| copy running-config startup-config | Salva configuração |

---

# Resumo

✅ Cisco utiliza uma interface de comandos chamada CLI.

✅ Existem diferentes modos de acesso.

✅ O comando **show** é usado para visualizar informações.

✅ O comando **configure terminal** permite alterar configurações.

✅ O comando **no shutdown** ativa interfaces.

✅ O comando **copy running-config startup-config** salva alterações.

---

# Curiosidade

No Cisco Packet Tracer, a prática com comandos CLI é muito importante porque simula equipamentos reais utilizados em empresas. Aprender esses comandos é uma das bases para certificações Cisco, como a **CCST Networking** e futuramente a **CCNA**.
