# 🧠 Endereçamento IP

## Mapa Mental

ENDEREÇAMENTO IP
│
├── O que é?
│   └── Endereço que identifica um dispositivo na rede.
│
├── Função
│   ├── Identificar dispositivos
│   ├── Permitir comunicação
│   └── Indicar origem e destino dos dados
│
├── Versões
│   ├── IPv4
│   └── IPv6
│
├── IPv4
│   ├── 32 bits
│   ├── 4 octetos
│   └── Ex.: 192.168.1.10
│
├── Componentes
│   ├── Endereço IP
│   ├── Máscara de sub-rede
│   ├── Gateway padrão
│   └── DNS
│
├── Tipos
│   ├── Público
│   ├── Privado
│   ├── Estático
│   └── Dinâmico
│
├── Classes
│   ├── A
│   ├── B
│   └── C
│
└── Quem fornece?
    ├── DHCP
    └── Configuração manual

---

# O que é?

O **Endereçamento IP** é um sistema utilizado para identificar cada dispositivo conectado a uma rede.

Assim como uma casa possui um endereço para receber correspondências, cada computador, celular ou impressora possui um **endereço IP** para enviar e receber informações.

---

# Explicando de forma simples

Imagine uma cidade.

🏠 Cada casa possui um endereço.

📮 O carteiro só consegue entregar a encomenda porque sabe onde cada casa está localizada.

Na rede acontece a mesma coisa.

O endereço IP informa exatamente onde os dados devem chegar.

Sem um endereço IP, os dispositivos não conseguem se comunicar.

---

# IPv4

É a versão mais utilizada atualmente.

Características:

- 32 bits
- Dividido em 4 grupos de números (octetos)
- Cada grupo varia de **0 a 255**

Exemplo:

192.168.1.10

---

# Como é formado um IPv4?

192 | 168 | 1 | 10

Cada parte recebe o nome de **octeto**.

Cada octeto possui 8 bits.

8 + 8 + 8 + 8 = **32 bits**

---

# IPv6

Foi criado porque os endereços IPv4 estão se esgotando.

Características:

- 128 bits
- Muito mais endereços disponíveis
- Utiliza números e letras

Exemplo:

2001:0db8:85a3:0000:0000:8a2e:0370:7334

---

# Componentes do Endereçamento

## Endereço IP

Identifica o dispositivo na rede.

Exemplo:

192.168.1.15

---

## Máscara de Sub-rede

Indica quais dispositivos pertencem à mesma rede.

Exemplo:

255.255.255.0

---

## Gateway Padrão

É o endereço do roteador.

Permite que o dispositivo se comunique com outras redes, como a Internet.

Exemplo:

192.168.1.1

---

## DNS

Traduz nomes de sites em endereços IP.

Exemplo:

www.google.com

↓

142.250.xxx.xxx

---

# Tipos de IP

## IP Público

- Visível na Internet.
- Fornecido pelo provedor de Internet (ISP).

Exemplo:

177.25.100.50

---

## IP Privado

Utilizado apenas dentro da rede local.

Faixas privadas:

Classe A

10.0.0.0 até 10.255.255.255

Classe B

172.16.0.0 até 172.31.255.255

Classe C

192.168.0.0 até 192.168.255.255

---

# IP Estático

É configurado manualmente.

Sempre permanece igual.

Exemplos de uso:

- Servidores
- Impressoras
- Câmeras IP

---

# IP Dinâmico

É atribuído automaticamente pelo servidor DHCP.

Pode mudar sempre que o dispositivo se conecta à rede.

---

# Classes de Endereços IPv4

Classe A

- Primeiro octeto: 1 a 126
- Grandes redes

Classe B

- Primeiro octeto: 128 a 191
- Redes médias

Classe C

- Primeiro octeto: 192 a 223
- Pequenas redes

---

# Como o computador recebe um IP?

Existem duas formas:

### Manual

O usuário configura:

- IP
- Máscara
- Gateway
- DNS

### Automática

O servidor **DHCP** fornece todas essas informações automaticamente.

---

# Exemplo Completo

Computador

IP: 192.168.1.20

Máscara:
255.255.255.0

Gateway:
192.168.1.1

DNS:
8.8.8.8

Assim, o computador consegue acessar outros dispositivos da rede e também a Internet.

---

# Resumo

✅ Identifica dispositivos na rede.

✅ IPv4 possui 32 bits.

✅ IPv6 possui 128 bits.

✅ O Gateway conecta a outras redes.

✅ O DNS traduz nomes de sites em IPs.

✅ O DHCP pode fornecer o IP automaticamente.

✅ O IP pode ser Público ou Privado.

✅ O IP pode ser Estático ou Dinâmico.

---

# Curiosidade

Quando você digita **www.google.com**, o computador não entende esse nome. Primeiro, ele consulta um servidor **DNS**, que informa o endereço IP correspondente. Só depois disso a conexão com o site é estabelecida.
