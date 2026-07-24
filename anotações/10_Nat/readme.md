# 🧠 NAT (Network Address Translation)

## Mapa Mental

NAT
│
├── O que é?
│   └── Tecnologia que traduz endereços IP privados em IP público.
│
├── Função
│   ├── Permitir acesso à Internet
│   ├── Economizar endereços IPv4
│   ├── Ocultar endereços internos da rede
│   └── Controlar a comunicação entre redes
│
├── Onde funciona?
│   └── Roteador
│
├── Utiliza
│   ├── IP privado
│   └── IP público
│
├── Tipos
│   ├── NAT Estático
│   ├── NAT Dinâmico
│   └── PAT (NAT Overload)
│
├── Tabela NAT
│   ├── IP interno
│   ├── Porta interna
│   ├── IP externo
│   └── Porta externa
│
└── Benefícios
    ├── Conserva IPv4
    ├── Aumenta segurança
    └── Permite vários dispositivos usando um único IP público

---

# O que é?

O **NAT (Network Address Translation)** é uma tecnologia utilizada pelo roteador para traduzir endereços IP privados em endereços IP públicos.

Ele permite que vários dispositivos dentro de uma rede doméstica ou empresarial acessem a Internet utilizando apenas um endereço IP público.

---

# Explicando de forma simples

Imagine um prédio.

🏢 O prédio possui apenas um endereço na rua.

Mas dentro dele existem vários apartamentos:

- Apartamento 101
- Apartamento 102
- Apartamento 103

Para quem está fora, todos pertencem ao mesmo endereço do prédio.

O NAT funciona da mesma forma:

🌐 Internet → vê apenas o IP público.

🏠 Rede interna → utiliza vários IPs privados.

---

# Por que o NAT existe?

O IPv4 possui uma quantidade limitada de endereços.

Com o crescimento da Internet, os endereços começaram a acabar.

O NAT ajudou permitindo que vários dispositivos compartilhassem um único endereço público.

---

# Como funciona?

Exemplo:

## Rede interna

Computador:

```
192.168.1.10
```

Celular:

```
192.168.1.20
```

Impressora:

```
192.168.1.30
```

Todos acessam a Internet através do mesmo IP público:

```
200.100.50.10
```

O roteador faz a tradução:

```
IP Privado
192.168.1.10

↓

IP Público
200.100.50.10
```

---

# Processo do NAT

1️⃣ Um dispositivo envia uma solicitação para a Internet.

2️⃣ O roteador recebe o pacote.

3️⃣ O NAT altera o endereço IP privado pelo IP público.

4️⃣ A informação chega ao servidor da Internet.

5️⃣ A resposta retorna ao roteador.

6️⃣ O NAT identifica qual dispositivo fez a solicitação e entrega a resposta correta.

---

# Tipos de NAT

## 1️⃣ NAT Estático

Um endereço privado é associado sempre ao mesmo endereço público.

Exemplo:

```
192.168.1.10

↓

200.50.10.5
```

Uso comum:

- Servidores
- Serviços que precisam ser acessados externamente

---

## 2️⃣ NAT Dinâmico

Os endereços privados recebem IPs públicos disponíveis em um grupo.

Exemplo:

Um dispositivo recebe temporariamente um IP público disponível.

---

## 3️⃣ PAT (Port Address Translation)

Também chamado de:

**NAT Overload**

É o tipo mais utilizado em redes domésticas.

Ele permite que vários dispositivos usem o mesmo IP público diferenciando as conexões pelas portas.

Exemplo:

```
Computador
192.168.1.10:5000

Celular
192.168.1.20:6000

↓

IP público:
200.100.50.10
```

---

# NAT e o Roteador

O NAT geralmente funciona dentro do roteador.

O roteador:

- Recebe os pacotes.
- Faz a tradução dos endereços.
- Encaminha para a Internet.

---

# NAT x DHCP

Apesar de trabalharem juntos, possuem funções diferentes:

| DHCP | NAT |
|---|---|
| Entrega IP aos dispositivos | Traduz IP privado para público |
| Funciona dentro da rede | Conecta rede interna à Internet |
| Configura dispositivos | Permite comunicação externa |

---

# NAT x IP Público e Privado

## IP Privado

Usado dentro da rede local.

Exemplos:

```
192.168.x.x
10.x.x.x
172.16.x.x até 172.31.x.x
```

---

## IP Público

Usado na Internet.

É fornecido pelo provedor de Internet (ISP).

---

# Exemplo prático

Em uma casa:

```
Notebook
192.168.1.5
      │
Celular
192.168.1.6
      │
      ▼
  Roteador com NAT
      │
      ▼
Internet
200.50.10.20
```

Para a Internet, parece que apenas o roteador está conectado.

---

# Resumo

✅ NAT significa Network Address Translation.

✅ Traduz IP privado em IP público.

✅ Funciona geralmente no roteador.

✅ Permite vários dispositivos compartilharem um IP público.

✅ Ajuda a economizar endereços IPv4.

✅ PAT é o tipo mais utilizado em redes domésticas.

---

# Curiosidade

Quando você acessa um site pelo celular ou computador em casa, o site não vê o IP privado do seu dispositivo. Ele vê o endereço IP público do seu roteador, porque o NAT realizou essa tradução antes da comunicação sair para a Internet.
