# Projeto Padrão - Apache Cassandra (NoSQL Orientado a Colunas)

Este projeto tem como objetivo criar um **SGDB NoSQL orientado a colunas** (Apache Cassandra) com um **projeto vazio** no Windows.

---

## Pré-requisitos

- Windows 10 ou superior
- OpenJDK 11 ou 8 instalado

---

## Passo 1 – Instalar o Java

1. Baixe o **OpenJDK 11**
   - [Oracle](https://www.oracle.com/br/java/technologies/javase/jdk11-archive-downloads.html)
2. Instale ou extraia o JDK em um diretório, por exemplo:  
   ```
   C:\Program Files\Java\jdk-11.0.20
   ```

---

## Passo 2 – Configurar a variável JAVA_HOME

1. Abra **Painel de Controle → Sistema → Configurações avançadas do sistema → Variáveis de Ambiente**
2. Em **Variáveis do sistema**, clique em **Path** e em **Editar**:
   - Clicar em Novo
   - Valor da variável: `C:\Program Files\Java\jdk-11.0.20\bin`
   - Necessário subir a váriavel até o topo
3. Clique em **OK** para salvar.

---

## Passo 3 – Verificar instalação do Java

Abra o **Prompt de Comando** ou **PowerShell** e digite:

```powershell
java -version
```

Deve aparecer algo como:

```
java version "11.0.20" 2024-08-01 LTS
```

---

## Passo 4 – Instalar o Apache Cassandra

1. Baixe a versão binária do Cassandra para Windows:  
   [Apache Cassandra Downloads](https://cassandra.apache.org/_/download.html)
2. Extraia o arquivo `.zip` em uma pasta, por exemplo:  
   ```
   C:\cassandra
   ```

---
## Passo 5 – Adicionar Cassandra ao Path
- Realizar os mesmos passos para adicionar o Java 11 nas variáveis de ambiente só que com o Cassandra

## Passo 6 – Rodar o Cassandra

1. Abra o **PowerShell** e navegue até a pasta `bin` do Cassandra:

```powershell
cd C:\cassandra\bin
```

2. Execute o Cassandra:

```powershell
cassandra -f
```

## Passo 7 – Conectar ao Cassandra (CQL Shell)

No **PowerShell**, digite:

```powershell
cqlsh
```

Isso abrirá o shell do Cassandra para executar comandos CQL.
