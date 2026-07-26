# 🧠 TCP (Transmission Control Protocol)

## Mapa Mental

TCP
│
├── O que é?
│   └── Protocolo que garante a entrega correta dos dados.
│
├── Características
│   ├── Confiável
│   ├── Orientado à conexão
│   ├── Verifica erros
│   └── Reenvia dados perdidos
│
├── Como funciona?
│   ├── Estabelece conexão
│   ├── Envia os dados
│   ├── Confirma o recebimento (ACK)
│   └── Encerra a conexão
│
├── Vantagens
│   ├── Dados chegam completos
│   ├── Maior segurança na transmissão
│   └── Evita perda de informações
│
├── Desvantagem
│   └── Mais lento que o UDP
│
└── Exemplos
    ├── HTTP
    ├── HTTPS
    ├── FTP
    ├── SMTP
    └── SSH

---

# O que é?

O **TCP (Transmission Control Protocol)** é um protocolo da camada de **Transporte** do modelo TCP/IP. Sua principal função é garantir que os dados cheguem ao destino corretamente, sem perdas e na ordem em que foram enviados.

---

# Explicando de forma simples

Imagine que você enviou um livro pelos Correios.

O TCP funciona como um serviço que:

📦 Conta todas as páginas antes do envio.

🚚 Entrega o livro.

📞 Pergunta ao destinatário se recebeu tudo corretamente.

🔄 Se alguma página estiver faltando, envia novamente.

Ou seja, o TCP se preocupa com a **confiabilidade da comunicação**.

---

# Como funciona?

1. Estabelece uma conexão entre os dispositivos.
2. Envia os dados em pequenos pacotes.
3. O destinatário confirma o recebimento através do **ACK (Acknowledgment)**.
4. Se algum pacote se perder, ele é reenviado.
5. Após o término da comunicação, a conexão é encerrada.

---

# Características

- ✔ Orientado à conexão.
- ✔ Confiável.
- ✔ Verifica erros.
- ✔ Garante a ordem dos pacotes.
- ✔ Reenvia pacotes perdidos.

---

# Vantagens

- Dados chegam completos.
- Evita perda de informações.
- Mantém a ordem correta dos pacotes.
- Muito utilizado em aplicações que exigem confiabilidade.

---

# Desvantagens

- Mais lento que o UDP.
- Consome mais recursos devido às confirmações de recebimento.

---

# Exemplos de uso

- 🌐 Navegação na Internet (HTTP/HTTPS)
- 📧 E-mails (SMTP, IMAP, POP3)
- 📁 Transferência de arquivos (FTP)
- 💻 Acesso remoto (SSH)

---

# Resumo

✅ Camada: Transporte

✅ Confiável

✅ Utiliza confirmação de recebimento (ACK)

✅ Reenvia pacotes perdidos

✅ Garante a ordem dos dados

✅ Mais lento que o UDP

---

# Curiosidade

O TCP é comparado a uma **carta registrada com Aviso de Recebimento (AR)**. O remetente só considera a entrega concluída quando recebe a confirmação de que o destinatário recebeu a carta.
