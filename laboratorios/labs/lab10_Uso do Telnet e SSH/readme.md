# Lab 09 - Usando Serviços FTP

## 🎯 Objetivo
Neste laboratório, utilizei o protocolo FTP para realizar o envio (upload) e o download de arquivos entre um computador cliente e um servidor FTP, compreendendo o funcionamento da transferência de arquivos em uma rede.

## 📂 Componentes
- 1 PC-A
- 1 Servidor FTP (ftp.pka)
- Cisco Packet Tracer

## ⚙️ Configuração
- Localizei o arquivo `sampleFile.txt` no computador cliente.
- Conectei-me ao servidor FTP utilizando o endereço IP `209.165.200.226`.
- Realizei a autenticação com as credenciais fornecidas.
- Enviei o arquivo para o servidor utilizando o protocolo FTP.
- Renomeei o arquivo armazenado no servidor.
- Baixei o arquivo novamente para o computador.
- Excluí o arquivo do servidor FTP.

## 🧪 Testes
- Listei os arquivos do computador utilizando o comando `dir`.
- Conectei ao servidor utilizando o comando `ftp 209.165.200.226`.
- Listei os arquivos do servidor com `dir`.
- Enviei o arquivo utilizando `put sampleFile.txt`.
- Renomeei o arquivo utilizando `rename`.
- Baixei o arquivo utilizando `get sampleFile_FTP.txt`.
- Excluí o arquivo do servidor utilizando `delete sampleFile_FTP.txt`.
- Finalizei a sessão FTP utilizando `quit`.

## 🛠️ Tecnologias utilizadas
- Cisco Packet Tracer
- FTP (File Transfer Protocol)
- TCP
- Command Prompt

## 💡 Habilidades desenvolvidas
- Utilização do protocolo FTP para transferência de arquivos.
- Conexão e autenticação em um servidor FTP.
- Upload e download de arquivos.
- Gerenciamento de arquivos em um servidor FTP.
- Utilização de comandos do Prompt de Comando.
- Compreensão da comunicação cliente-servidor utilizando FTP.

## ✅ Verificação Final
Verifiquei que o protocolo FTP permite realizar operações de upload, download, renomeação e exclusão de arquivos em um servidor remoto, utilizando comandos específicos após a autenticação do usuário.
