# 🧠 Tabela de Roteamento (Routing Table)

## Mapa Mental

TABELA DE ROTEAMENTO
│
├── O que é?
│   └── Lista de caminhos que o roteador utiliza para encaminhar pacotes.
│
├── Função
│   ├── Identificar redes conhecidas
│   ├── Escolher o melhor caminho
│   ├── Encaminhar pacotes
│   └── Conectar diferentes redes
│
├── Encontrada em
│   ├── Roteadores
│   └── Computadores (tabela de rotas)
│
├── Informações armazenadas
│   ├── Rede de destino
│   ├── Máscara de sub-rede
│   ├── Próximo salto (Next Hop)
│   ├── Interface de saída
│   └── Tipo da rota
│
├── Tipos de rotas
│   ├── Conectada diretamente (C)
│   ├── Estática (S)
│   ├── Dinâmica (D, O, R...)
│   └── Rota padrão (Gateway)
│
└── Protocolos de roteamento
    ├── RIP
    ├── OSPF
    ├── EIGRP
    └── BGP

---

# O que é uma Tabela de Roteamento?

A **Tabela de Roteamento** é uma tabela que contém informações sobre os caminhos que um roteador conhece para enviar dados até outras redes.

Ela funciona como um **mapa de caminhos**.

O roteador consulta essa tabela sempre que precisa decidir para onde enviar um pacote.

---

# Explicando de forma simples

Imagine um GPS.

🚗 Você informa o destino.

📍 O GPS verifica os caminhos disponíveis.

🛣️ Ele escolhe a melhor rota.

O roteador faz algo parecido:

- Recebe um pacote.
- Verifica o endereço IP de destino.
- Consulta sua tabela.
- Escolhe o caminho.
- Envia o pacote.

---

# Como funciona?

Exemplo:

Um computador deseja acessar um servidor:

```
Computador
192.168.1.10

↓

Roteador

↓

Servidor
8.8.8.8
```

O roteador verifica:

"Conheço a rede 8.8.8.0?"

Se sim:

➡️ Encaminha pelo caminho registrado.

Se não:

➡️ Procura uma rota padrão.

---

# Informações de uma tabela de roteamento

Uma tabela possui:

## Rede de destino

Indica para qual rede o pacote deve ir.

Exemplo:

```
192.168.2.0/24
```

---

## Máscara de rede

Define o tamanho da rede.

Exemplo:

```
255.255.255.0
```

---

## Próximo salto (Next Hop)

É o próximo roteador que receberá o pacote.

Exemplo:

```
192.168.1.254
```

---

## Interface de saída

Indica por qual porta o pacote deve sair.

Exemplo:

```
GigabitEthernet0/1
```

---

## Métrica

É um valor usado para escolher o melhor caminho.

Pode considerar:

- Distância.
- Velocidade.
- Quantidade de saltos.
- Custo da rota.

---

# Tipos de rotas

## 1️⃣ Rota Diretamente Conectada (C)

É uma rede que está ligada diretamente ao roteador.

Exemplo:

Um computador conectado na porta do roteador.

Representação:

```
C 192.168.1.0/24
```

---

## 2️⃣ Rota Estática (S)

É configurada manualmente pelo administrador.

O administrador informa o caminho que deve ser usado.

Exemplo:

```
ip route 192.168.2.0 255.255.255.0 10.0.0.2
```

Vantagens:

✔ Simples.

✔ Controle maior.

Desvantagens:

❌ Difícil em redes muito grandes.

---

## 3️⃣ Rota Dinâmica

É aprendida automaticamente através de protocolos de roteamento.

Exemplos:

- RIP
- OSPF
- EIGRP
- BGP

Vantagens:

✔ Se adapta às mudanças.

✔ Melhor para redes grandes.

---

## 4️⃣ Rota Padrão (Default Route)

É utilizada quando o roteador não conhece o destino.

Representação:

```
0.0.0.0/0
```

Normalmente aponta para a Internet.

Exemplo:

Computador → Roteador → Provedor → Internet

---

# Exemplo de uma tabela

| Código | Rede destino | Próximo salto |
|---|---|---|
| C | 192.168.1.0/24 | Direto |
| S | 192.168.2.0/24 | 10.0.0.2 |
| D | 10.0.0.0/8 | 192.168.1.2 |
| S* | 0.0.0.0/0 | Gateway Internet |

---

# Códigos comuns no Cisco

| Código | Significado |
|---|---|
| C | Connected (Conectada diretamente) |
| L | Local |
| S | Static (Estática) |
| D | EIGRP |
| O | OSPF |
| R | RIP |
| * | Rota candidata padrão |

---

# Comandos Cisco importantes

## Visualizar tabela de roteamento

```
show ip route
```

Mostra todas as rotas conhecidas pelo roteador.

---

## Criar uma rota estática

```
ip route rede máscara próximo_salto
```

Exemplo:

```
ip route 192.168.2.0 255.255.255.0 10.0.0.2
```

---

# Relação com outros conceitos

## Switch

Trabalha com:

➡️ MAC

Camada 2

---

## Roteador

Trabalha com:

➡️ IP

Camada 3

---

## Tabela de Roteamento

Ajuda o roteador a decidir:

➡️ Para onde enviar o pacote.

---

# Resumo

✅ A tabela de roteamento é o mapa do roteador.

✅ Contém caminhos para diferentes redes.

✅ Usa endereços IP para tomar decisões.

✅ Pode possuir rotas conectadas, estáticas e dinâmicas.

✅ A rota padrão leva o tráfego para destinos desconhecidos.

✅ O comando Cisco para visualizar é:

```
show ip route
```

---

# Curiosidade

A Internet inteira funciona graças a milhões de tabelas de roteamento. Cada roteador toma decisões independentes, enviando os pacotes de um ponto ao outro até chegarem ao destino final.
