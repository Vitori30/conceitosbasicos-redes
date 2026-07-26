# 🧠 Portas e Protocolos de Rede

## Mapa Mental

PORTAS E PROTOCOLOS
│
├── Protocolo
│   ├── Conjunto de regras de comunicação
│   ├── Define como os dados serão enviados
│   └── Permite comunicação entre dispositivos
│
├── Porta de Rede
│   ├── Identifica serviços e aplicações
│   ├── Funciona como uma "entrada" para comunicação
│   └── Trabalha junto com o endereço IP
│
├── Comunicação
│   ├── IP → identifica o dispositivo
│   ├── Porta → identifica o serviço
│   └── Protocolo → define as regras
│
├── Principais Protocolos
│   ├── HTTP
│   ├── HTTPS
│   ├── FTP
│   ├── SSH
│   ├── DNS
│   ├── DHCP
│   ├── SMTP
│   ├── POP3
│   └── IMAP
│
└── Protocolos de Transporte
    ├── TCP
    └── UDP

---

# O que são protocolos?

Os **protocolos de rede** são conjuntos de regras que permitem que dispositivos consigam se comunicar.

Eles definem:

- Como os dados serão enviados.
- Como serão recebidos.
- Como os erros serão tratados.
- Como os dispositivos irão entender as informações.

---

# Explicando de forma simples

Imagine uma conversa entre pessoas de países diferentes.

Para elas se entenderem, precisam seguir uma regra de comunicação, como um idioma.

O protocolo funciona como esse idioma da rede.

Sem protocolos, os computadores não conseguiriam trocar informações.

---

# O que são portas de rede?

As **portas de rede** são números utilizados para identificar qual serviço ou aplicação deve receber determinada informação.

Um computador pode executar vários serviços ao mesmo tempo.

A porta informa para onde o dado deve ir.

---

# Explicando de forma simples

Imagine um prédio:

🏢 O endereço do prédio = Endereço IP

🚪 O número do apartamento = Porta

👤 O morador = Serviço

O IP informa qual dispositivo receberá.

A porta informa qual aplicação deve receber.

---

# Relação entre IP, Porta e Protocolo

Exemplo:

Acessar um site:

```
IP:
142.250.xxx.xxx

Porta:
443

Protocolo:
HTTPS
```

Significa:

"Enviar dados para esse computador, usando a porta 443, através do protocolo HTTPS."

---

# Principais Portas e Protocolos

## 🌐 HTTP

**HyperText Transfer Protocol**

Porta:

```
80 TCP
```

Função:

- Acessar páginas da Web.
- Transferir informações entre navegador e servidor.

Exemplo:

```
http://site.com
```

---

## 🔒 HTTPS

**HyperText Transfer Protocol Secure**

Porta:

```
443 TCP
```

Função:

- Comunicação segura na Internet.
- Utiliza criptografia.

Exemplo:

```
https://site.com
```

---

## 📁 FTP

**File Transfer Protocol**

Portas:

```
20 e 21 TCP
```

Função:

- Transferência de arquivos.

Exemplo:

Enviar arquivos para um servidor.

---

## 💻 SSH

**Secure Shell**

Porta:

```
22 TCP
```

Função:

- Acesso remoto seguro.
- Administração de servidores.

---

## 🌎 DNS

**Domain Name System**

Porta:

```
53 UDP/TCP
```

Função:

- Traduz nomes de domínio em endereços IP.

Exemplo:

```
google.com
↓
Endereço IP
```

---

## 📡 DHCP

**Dynamic Host Configuration Protocol**

Portas:

```
67 UDP (Servidor)
68 UDP (Cliente)
```

Função:

- Entregar configurações de rede automaticamente.

Fornece:

- IP.
- Máscara.
- Gateway.
- DNS.

---

## 📧 SMTP

**Simple Mail Transfer Protocol**

Portas:

```
25
587
```

Função:

- Envio de e-mails.

---

## 📥 POP3

**Post Office Protocol**

Porta:

```
110 TCP
```

Função:

- Receber e baixar e-mails.

---

## 📬 IMAP

**Internet Message Access Protocol**

Porta:

```
143 TCP
```

Função:

- Acessar e-mails mantendo sincronização com o servidor.

---

# TCP e UDP

Os protocolos de transporte são responsáveis pela comunicação entre aplicações.

---

# TCP

**Transmission Control Protocol**

Características:

✔ Confiável.

✔ Confirma recebimento.

✔ Reenvia dados perdidos.

✔ Mantém a ordem dos pacotes.

Exemplos:

- HTTPS.
- FTP.
- SSH.

---

# UDP

**User Datagram Protocol**

Características:

✔ Mais rápido.

✔ Não confirma recebimento.

✔ Menor controle.

Exemplos:

- Jogos online.
- Streaming.
- Chamadas de vídeo.

---

# Tabela de resumo

| Protocolo | Porta | Transporte | Função |
|---|---|---|---|
| HTTP | 80 | TCP | Navegação Web |
| HTTPS | 443 | TCP | Web segura |
| FTP | 20/21 | TCP | Transferência de arquivos |
| SSH | 22 | TCP | Acesso remoto |
| DNS | 53 | UDP/TCP | Resolver nomes |
| DHCP | 67/68 | UDP | Configurar IP |
| SMTP | 25/587 | TCP | Enviar e-mail |
| POP3 | 110 | TCP | Receber e-mail |
| IMAP | 143 | TCP | Sincronizar e-mail |

---

# Comandos para verificar portas

## Windows

Ver conexões e portas abertas:

```
netstat -ano
```

Ver configuração de rede:

```
ipconfig
```

Testar comunicação:

```
ping endereço
```

---

# Resumo

✅ Protocolos são regras de comunicação.

✅ Portas identificam serviços e aplicações.

✅ O IP identifica o dispositivo.

✅ TCP garante confiabilidade.

✅ UDP prioriza velocidade.

✅ Cada serviço utiliza uma porta específica.

---

# Curiosidade

Um computador possui **65.535 portas disponíveis**. Isso permite que vários serviços funcionem simultaneamente usando o mesmo endereço IP, mas em portas diferentes.
