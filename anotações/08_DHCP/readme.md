# 🧠 DHCP (Dynamic Host Configuration Protocol)

## Mapa Mental

DHCP
│
├── O que é?
│   └── Protocolo que configura dispositivos automaticamente na rede.
│
├── Função
│   ├── Entregar endereço IP
│   ├── Informar máscara de sub-rede
│   ├── Informar gateway padrão
│   └── Informar servidor DNS
│
├── Funcionamento
│   └── Processo DORA
│       ├── Discover
│       ├── Offer
│       ├── Request
│       └── Acknowledge
│
├── Utiliza
│   ├── Servidor DHCP
│   └── Cliente DHCP
│
├── Porta
│   ├── UDP 67 → Servidor
│   └── UDP 68 → Cliente
│
├── Tipos de configuração
│   ├── Automática
│   ├── Dinâmica
│   └── Manual (Reserva DHCP)
│
└── Problemas comuns
    ├── Falha no DHCP
    ├── IP 169.254.x.x (APIPA)
    └── Sem acesso à rede

---

# O que é?

O **DHCP (Dynamic Host Configuration Protocol)** é um protocolo responsável por configurar automaticamente os dispositivos dentro de uma rede.

Ele evita que seja necessário configurar manualmente cada computador, celular ou equipamento conectado.

---

# Explicando de forma simples

Imagine uma escola onde cada aluno precisa receber um número de identificação.

Em vez de o professor entregar manualmente um número para cada aluno, existe uma pessoa responsável que distribui automaticamente os números.

O **DHCP faz esse papel na rede**.

Quando um dispositivo se conecta, ele recebe automaticamente:

📌 Endereço IP  
📌 Máscara de sub-rede  
📌 Gateway padrão  
📌 Servidor DNS  

---

# Como funciona o DHCP?

O funcionamento acontece através do processo chamado **DORA**.

## 1️⃣ Discover (Descoberta)

O dispositivo entra na rede e pergunta:

"Existe algum servidor DHCP disponível?"

Essa mensagem é enviada como **Broadcast**.

---

## 2️⃣ Offer (Oferta)

O servidor DHCP responde:

"Eu posso fornecer este endereço IP para você."

Exemplo:

```
IP: 192.168.1.50
Máscara: 255.255.255.0
Gateway: 192.168.1.1
```

---

## 3️⃣ Request (Solicitação)

O dispositivo informa:

"Eu aceito esse endereço IP."

---

## 4️⃣ Acknowledge (Confirmação)

O servidor confirma:

"Esse IP está reservado para você."

A partir desse momento o dispositivo pode se comunicar na rede.

---

# Informações fornecidas pelo DHCP

## Endereço IP

Identifica o dispositivo na rede.

Exemplo:

```
192.168.1.20
```

---

## Máscara de Sub-rede

Define qual parte do IP representa a rede e qual representa o dispositivo.

Exemplo:

```
255.255.255.0
```

---

## Gateway Padrão

Indica o caminho para outras redes.

Normalmente é o endereço do roteador.

Exemplo:

```
192.168.1.1
```

---

## DNS

Informa qual servidor será usado para transformar nomes de sites em endereços IP.

Exemplo:

```
www.google.com
```

↓

```
142.250.xxx.xxx
```

---

# Servidor DHCP

É o equipamento responsável por entregar as configurações de rede.

Pode estar em:

- Roteadores domésticos.
- Servidores empresariais.
- Equipamentos de rede.

---

# Cliente DHCP

É qualquer dispositivo que solicita uma configuração de rede.

Exemplos:

- Computador.
- Notebook.
- Celular.
- Impressora.
- Smart TV.

---

# Portas utilizadas

O DHCP utiliza o protocolo **UDP**.

## Servidor DHCP

```
Porta 67
```

## Cliente DHCP

```
Porta 68
```

---

# Tipos de atribuição de IP

## Automática

O DHCP entrega um IP disponível.

Exemplo:

Computador recebe:

```
192.168.1.10
```

---

## Dinâmica

O IP possui um tempo de uso chamado **concessão (Lease)**.

Após esse período, o endereço pode ser renovado ou alterado.

---

## Reserva DHCP

O administrador define que determinado dispositivo sempre receberá o mesmo IP.

Muito usado em:

- Impressoras.
- Servidores.
- Câmeras IP.

---

# Problema comum: APIPA

Quando um computador não consegue encontrar um servidor DHCP, ele pode gerar automaticamente um endereço:

```
169.254.x.x
```

Esse endereço é chamado de **APIPA**.

Quando isso acontece, normalmente significa:

❌ Falha na comunicação com o DHCP.

Possíveis causas:

- Cabo desconectado.
- Wi-Fi com problema.
- Servidor DHCP desligado.
- Configuração incorreta.

---

# DHCP x IP Estático

| DHCP | IP Estático |
|---|---|
| Automático | Manual |
| Mais fácil de administrar | Requer configuração |
| Pode mudar | Permanece igual |
| Usado em computadores comuns | Usado em servidores |

---

# Exemplo prático

Você chega em casa e conecta o celular no Wi-Fi.

O processo é:

📱 Celular solicita configuração.

⬇️

📡 Roteador (servidor DHCP) entrega:

- IP
- Máscara
- Gateway
- DNS

⬇️

🌐 Celular acessa a Internet.

---

# Resumo

✅ DHCP configura dispositivos automaticamente.

✅ Entrega IP, máscara, gateway e DNS.

✅ Utiliza o processo DORA.

✅ Usa UDP 67 e 68.

✅ Evita configurações manuais.

✅ Falha no DHCP pode gerar IP 169.254.x.x (APIPA).

---

# Curiosidade

Em uma rede grande, como uma empresa, o DHCP permite configurar centenas ou milhares de dispositivos sem que um administrador precise configurar cada máquina individualmente.
