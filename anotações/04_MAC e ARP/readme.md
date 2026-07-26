# 🧠 MAC e ARP

## Mapa Mental

MAC e ARP
│
├── Endereço MAC
│   ├── Identifica o dispositivo
│   ├── É físico
│   ├── Gravado pelo fabricante
│   └── Atua na Camada de Enlace
│
├── ARP
│   ├── Descobre o endereço MAC
│   ├── Usa o endereço IP
│   ├── Funciona na rede local
│   └── Atualiza a tabela ARP
│
├── Relação
│   ├── IP identifica onde está o dispositivo
│   └── MAC identifica qual é o dispositivo
│
└── Equipamentos
    ├── Switch → utiliza MAC
    └── Roteador → utiliza IP

---

# O que é o endereço MAC?

O **MAC (Media Access Control)** é um endereço físico que identifica **cada placa de rede** de um dispositivo.

Ele é único e é gravado pelo fabricante, funcionando como um "CPF" da placa de rede.

O endereço MAC pertence à **Camada 2 (Enlace)** do Modelo OSI.

---

# Explicando de forma simples

Imagine um condomínio.

- O **endereço IP** é o número do apartamento.
- O **endereço MAC** é o nome da pessoa que mora naquele apartamento.

Para entregar uma encomenda, o entregador precisa saber:

- Em qual apartamento entregar (IP).
- Quem mora lá (MAC).

Na rede acontece a mesma coisa.

---

# Como é um endereço MAC?

É formado por **48 bits**, representados por **12 caracteres hexadecimais**, separados por dois-pontos (:) ou hífens (-).

Exemplo:

```
00:1A:2B:3C:4D:5E
```

Cada equipamento possui um MAC diferente.

---

# Características do MAC

- ✔ Único para cada placa de rede.
- ✔ Gravado pelo fabricante.
- ✔ Não depende da Internet.
- ✔ Utilizado dentro da rede local (LAN).
- ✔ Trabalha na Camada de Enlace.

---

# O que é o ARP?

**ARP (Address Resolution Protocol)** é o protocolo responsável por descobrir o **endereço MAC** de um dispositivo utilizando o seu **endereço IP**.

Ou seja:

➡️ O computador sabe o IP.

➡️ O ARP descobre qual é o MAC correspondente.

---

# Como o ARP funciona?

Imagine que o computador deseja enviar dados para o IP:

```
192.168.1.20
```

Mas ele não conhece o MAC desse dispositivo.

Então acontece o seguinte:

### 1️⃣ O computador envia uma mensagem para toda a rede (Broadcast)

"Quem possui o IP 192.168.1.20?"

---

### 2️⃣ O dispositivo responde

"Sou eu!"

"Inclusive meu MAC é:

```
00:1A:2B:3C:4D:5E
```

---

### 3️⃣ O computador salva essa informação

Ela fica armazenada na **Tabela ARP (ARP Cache)**.

Assim, nas próximas comunicações não será necessário perguntar novamente.

---

# O que é Broadcast?

Broadcast significa enviar uma mensagem para **todos os dispositivos da rede**.

Somente o equipamento que possui o IP procurado responderá.

---

# Onde o ARP funciona?

O ARP funciona **apenas dentro da rede local (LAN)**.

Ele não atravessa roteadores.

---

# Relação entre IP, MAC e ARP

Imagine que você quer entregar uma encomenda.

📍 Endereço da casa = IP

👤 Nome do morador = MAC

📞 Perguntar quem mora naquele endereço = ARP

Depois de descobrir quem mora lá, a entrega pode ser realizada.

---

# Equipamentos que utilizam

## Switch

Utiliza o endereço **MAC** para encaminhar os quadros ao dispositivo correto.

---

## Roteador

Utiliza o endereço **IP** para encaminhar os pacotes entre redes diferentes.

---

# Resumo

✅ MAC identifica o dispositivo.

✅ IP identifica onde o dispositivo está na rede.

✅ ARP descobre o MAC usando o IP.

✅ O ARP funciona apenas na rede local.

✅ O Switch trabalha principalmente com MAC.

✅ O Roteador trabalha principalmente com IP.

---

# Curiosidade

Você pode visualizar a tabela ARP do seu computador usando o comando:

```bash
arp -a
```

Esse comando mostra os endereços **IP** e os respectivos **MAC** dos dispositivos que o computador já conhece na rede.
