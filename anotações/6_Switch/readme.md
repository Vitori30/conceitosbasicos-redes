# 🧠 Switch

## Mapa Mental

SWITCH
│
├── O que é?
│   └── Equipamento que conecta dispositivos em uma rede local (LAN).
│
├── Função
│   ├── Receber quadros (Frames)
│   ├── Ler o endereço MAC
│   ├── Encontrar o destino
│   └── Enviar apenas para o dispositivo correto
│
├── Trabalha na
│   └── Camada 2 (Enlace)
│
├── Utiliza
│   └── Endereço MAC
│
├── Conecta
│   ├── Computadores
│   ├── Impressoras
│   ├── Servidores
│   ├── Access Points
│   └── Roteadores
│
├── Tabela MAC
│   ├── Aprende automaticamente
│   └── Armazena os endereços dos dispositivos
│
├── Vantagens
│   ├── Comunicação mais rápida
│   ├── Menos colisões
│   ├── Melhor desempenho
│   └── Maior eficiência
│
└── Diferença
    ├── Hub → Envia para todos
    └── Switch → Envia apenas para o destino

---

# O que é?

O **Switch** é um equipamento de rede utilizado para conectar vários dispositivos em uma **rede local (LAN)**.

Sua principal função é receber os dados e encaminhá-los **somente para o dispositivo correto**, tornando a comunicação mais rápida e eficiente.

---

# Explicando de forma simples

Imagine uma escola.

Cada sala possui um número.

Quando chega uma encomenda para a sala 5, o funcionário leva apenas para a sala 5.

Ele não entra em todas as salas perguntando quem é o dono.

O **Switch funciona exatamente assim**.

Ele sabe onde cada dispositivo está conectado e envia os dados apenas para quem deve recebê-los.

---

# Como funciona?

Quando um computador envia dados:

1. O Switch recebe o quadro (Frame).
2. Lê o endereço **MAC** de destino.
3. Consulta sua **Tabela MAC**.
4. Descobre em qual porta o dispositivo está conectado.
5. Envia o quadro somente para aquela porta.

---

# O que é a Tabela MAC?

A **Tabela MAC** é uma lista criada automaticamente pelo Switch.

Ela registra:

- Endereço MAC
- Porta onde o dispositivo está conectado

Exemplo:

| Endereço MAC | Porta |
|--------------|-------|
| 00:1A:2B:3C:4D:5E | Fa0/1 |
| 08:7F:AA:11:22:33 | Fa0/2 |
| 10:AB:CD:44:55:66 | Fa0/3 |

Assim, o Switch sabe exatamente para onde enviar cada quadro.

---

# Em qual camada o Switch trabalha?

O Switch atua principalmente na **Camada 2 (Enlace)** do Modelo OSI.

Nessa camada ele utiliza o **endereço MAC** para identificar os dispositivos.

> Alguns switches mais avançados (Camada 3) também podem realizar funções de roteamento utilizando endereços IP.

---

# Equipamentos que podem ser conectados

- 💻 Computadores
- 🖨️ Impressoras
- 🖥️ Servidores
- 📡 Access Points
- 🌐 Roteadores
- 📷 Câmeras IP

---

# Switch x Hub

## Hub

- Envia os dados para **todos** os dispositivos.
- Gera mais tráfego na rede.
- É mais lento.
- Atualmente é pouco utilizado.

## Switch

- Envia os dados apenas para o dispositivo correto.
- Reduz o tráfego da rede.
- É mais rápido.
- É o equipamento mais utilizado nas redes locais.

---

# Vantagens

- ✔ Comunicação mais rápida.
- ✔ Reduz colisões.
- ✔ Melhor desempenho da rede.
- ✔ Utiliza a largura de banda de forma mais eficiente.
- ✔ Fácil expansão da rede.

---

# Exemplo prático

Imagine uma rede com quatro computadores.

```
PC1
   │
PC2 ─── Switch ─── Impressora
   │
PC3
   │
PC4
```

Se o **PC1** enviar um documento para a impressora:

- O Switch identifica o endereço MAC da impressora.
- Encaminha os dados apenas para ela.
- Os demais computadores não recebem esse tráfego.

---

# Resumo

✅ Conecta dispositivos em uma rede local.

✅ Trabalha principalmente na Camada 2 (Enlace).

✅ Utiliza endereços MAC.

✅ Aprende automaticamente onde cada dispositivo está conectado.

✅ Encaminha os dados apenas para o destino correto.

---

# Curiosidade

O Switch "aprende" os endereços MAC automaticamente. Sempre que um dispositivo envia um quadro, ele registra o endereço MAC e a porta correspondente em sua tabela. Assim, quanto mais a rede é utilizada, mais eficiente o Switch se torna no encaminhamento dos dados.
