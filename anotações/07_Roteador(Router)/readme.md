# 🧠 Roteador (Router)

## Mapa Mental

ROTEADOR
│
├── O que é?
│   └── Equipamento que conecta redes diferentes.
│
├── Função principal
│   ├── Escolher o melhor caminho para os dados
│   ├── Encaminhar pacotes entre redes
│   └── Conectar a rede local à Internet
│
├── Trabalha na
│   └── Camada 3 - Rede (Modelo OSI)
│
├── Utiliza
│   └── Endereço IP
│
├── Possui
│   ├── Tabela de roteamento
│   ├── Endereço IP
│   └── Interfaces de rede
│
├── Conecta
│   ├── Redes locais (LAN)
│   ├── Internet (WAN)
│   ├── Filiais
│   └── Diferentes redes
│
├── Serviços comuns
│   ├── DHCP
│   ├── NAT
│   ├── Firewall
│   └── Wi-Fi
│
└── Diferença
    ├── Switch → conecta dispositivos na mesma rede
    └── Roteador → conecta redes diferentes

---

# O que é?

O **Roteador** é um equipamento responsável por conectar diferentes redes e encaminhar os dados até o destino correto.

Ele funciona como um "guia" da rede, analisando os endereços IP e escolhendo o melhor caminho para os pacotes chegarem ao destino.

---

# Explicando de forma simples

Imagine uma cidade com vários bairros.

🏠 Uma casa representa um dispositivo.

🏘️ Um bairro representa uma rede.

🛣️ As ruas representam os caminhos possíveis.

O roteador funciona como um GPS:

- Ele sabe onde cada rede está.
- Escolhe o melhor caminho.
- Encaminha a informação até o destino.

---

# Como funciona?

Quando um dispositivo deseja acessar a Internet:

Exemplo:

Computador:
```
192.168.1.10
```

Quer acessar um servidor:

```
8.8.8.8
```

O processo é:

1️⃣ O computador envia o pacote para o Gateway Padrão.

2️⃣ O roteador recebe o pacote.

3️⃣ Analisa o endereço IP de destino.

4️⃣ Consulta sua tabela de roteamento.

5️⃣ Encaminha o pacote pelo melhor caminho.

---

# Camada do Modelo OSI

O roteador trabalha principalmente na:

## 3️⃣ Camada de Rede

Responsável por:

- Endereçamento IP.
- Escolha de caminhos.
- Encaminhamento de pacotes.

---

# O que o roteador utiliza?

## Endereço IP

O roteador trabalha com endereços IP para identificar redes e dispositivos.

Exemplo:

Rede local:

```
192.168.1.0/24
```

Internet:

```
200.100.50.10
```

---

# Tabela de Roteamento

A tabela de roteamento é uma lista que informa ao roteador:

- Quais redes ele conhece.
- Qual caminho utilizar.
- Para onde enviar os pacotes.

Exemplo:

| Rede destino | Próximo salto |
|---|---|
| 192.168.1.0 | Direto |
| 10.0.0.0 | Roteador vizinho |
| 0.0.0.0 | Internet |

---

# Gateway Padrão

O gateway padrão é o endereço do roteador usado pelos dispositivos para sair da rede local.

Exemplo:

Computador:

```
IP: 192.168.1.20
```

Gateway:

```
192.168.1.1
```

Quando o computador precisa acessar outra rede, ele envia os dados para o roteador.

---

# Funções comuns do roteador

## DHCP

Distribui endereços IP automaticamente para os dispositivos.

Exemplo:

Um celular conecta no Wi-Fi e recebe um IP.

---

## NAT

Traduz endereços privados em públicos.

Exemplo:

Rede interna:

```
192.168.1.10
```

↓

Internet:

```
200.50.10.5
```

Permite que vários dispositivos compartilhem uma conexão com a Internet.

---

## Firewall

Ajuda a controlar o tráfego da rede e bloquear acessos indesejados.

---

# Roteador x Switch

| Switch | Roteador |
|---|---|
| Conecta dispositivos na mesma rede | Conecta redes diferentes |
| Usa MAC | Usa IP |
| Camada 2 | Camada 3 |
| Rede local | Comunicação entre redes |

---

# Exemplo prático

Em uma casa:

```
Celular
   │
Notebook ─── Roteador ─── Internet
   │
Smart TV
```

O roteador:

- Cria a rede Wi-Fi.
- Entrega IPs.
- Permite acesso à Internet.
- Controla o tráfego.

---

# Resumo

✅ Conecta redes diferentes.

✅ Trabalha na Camada 3 do Modelo OSI.

✅ Utiliza endereços IP.

✅ Escolhe caminhos para os pacotes.

✅ Possui uma tabela de roteamento.

✅ É o equipamento que normalmente conecta uma rede doméstica ou empresarial à Internet.

---

# Curiosidade

Um roteador doméstico geralmente reúne várias funções em um único equipamento: roteador, switch, ponto de acesso Wi-Fi, servidor DHCP e recursos básicos de segurança.
