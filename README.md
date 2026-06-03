# 🔍 Missão 03 - Operação Deep Scan

## 📖 Sobre a Atividade

Esta atividade teve como objetivo desenvolver uma aplicação de console em C# utilizando .NET, simulando um processo de análise de sistema ("Deep Scan") enquanto aplica conceitos de Interação Humano-Computador (IHC), especificamente a **1ª Heurística de Nielsen: Visibilidade do Status do Sistema**.

O programa fornece feedback contínuo ao usuário durante a execução, informando em tempo real as etapas do processamento e evitando a sensação de travamento ou falta de resposta do sistema.

---

## 🎯 Objetivos

* Criar uma aplicação Console utilizando .NET CLI.
* Aplicar a Heurística de Nielsen "Visibilidade do Status do Sistema".
* Simular um processo de carregamento utilizando `Thread.Sleep()`.
* Melhorar a experiência do usuário através de feedback visual.
* Demonstrar a importância da comunicação entre sistema e usuário.

---

## 🛠️ Tecnologias Utilizadas

* C#
* .NET SDK
* Visual Studio Code
* Terminal (CMD / PowerShell)

---

## 📂 Estrutura do Projeto

```text
una-ihcux-lista03/
│
├── ScannerExpert/
│   ├── Program.cs
│   ├── ScannerExpert.csproj
│   └── obj/
│
├── minha-evidencia.png
└── README.md
```

---

## 🚀 Funcionalidades

O sistema simula uma análise de hardware executando as seguintes etapas:

* Verificação da CPU
* Leitura da memória RAM
* Sincronização do SDK
* Validação de permissões
* Finalização da análise

Durante cada etapa, o usuário recebe mensagens de progresso exibidas diretamente no terminal.

---

## 💡 Conceito de UX Aplicado

### 1ª Heurística de Nielsen

**Visibilidade do Status do Sistema**

O sistema deve manter o usuário informado sobre o que está acontecendo, fornecendo feedback apropriado em tempo razoável.

No projeto, isso é implementado através das mensagens:

```text
[PROCESSANDO] Verificando CPU...
[PROCESSANDO] Lendo Memória RAM...
[PROCESSANDO] Sincronizando SDK...
```

Essas informações permitem que o usuário saiba que o programa está funcionando corretamente e executando tarefas em segundo plano.

---

## 🔧 Recursos Utilizados

### Thread.Sleep()

Utilizado para simular o tempo necessário para processamento.

Exemplo:

```csharp
Thread.Sleep(1500);
```

Neste caso, o programa aguarda 1,5 segundo antes de avançar para a próxima etapa.

### Carriage Return (\r)

Permite atualizar a mesma linha do terminal sem criar várias linhas repetidas.

Exemplo:

```csharp
Console.Write("\r[PROCESSANDO] Verificando CPU...");
```

Isso torna a interface mais limpa e organizada.

---

## ▶️ Como Executar

1. Abra o terminal.
2. Navegue até a pasta do projeto.

```bash
cd ScannerExpert
```

3. Execute a aplicação.

```bash
dotnet run
```

4. Observe o progresso da análise exibido em tempo real.

---

## 📸 Evidência de Execução

Adicionar abaixo a captura de tela mostrando o sistema durante a fase de processamento.

```markdown
![Evidência de Execução](./minha-evidencia.png)
```

---

## 🧠 Reflexão sobre UX

### Pergunta

**Se o programa demorasse 10 segundos para finalizar, mas ficasse com a tela totalmente parada (em branco), sem as mensagens de "[PROCESSANDO]", o que o usuário provavelmente pensaria? Como a visibilidade de status melhora a Experiência do Usuário (UX)?**

### Resposta

Se o sistema permanecesse em silêncio durante os 10 segundos, o usuário poderia acreditar que o programa travou, apresentou erro ou deixou de responder. Essa incerteza gera ansiedade, frustração e diminui a confiança no software.

A visibilidade de status melhora a experiência do usuário porque fornece feedback constante sobre o andamento das tarefas. Mesmo quando o processamento leva algum tempo, o usuário entende que o sistema continua funcionando normalmente e sabe exatamente em qual etapa a operação se encontra.

---

## 📚 Aprendizados

Durante esta atividade foi possível aprender:

* Criação de projetos utilizando .NET CLI.
* Utilização de `Thread.Sleep()` para simular processamento.
* Atualização dinâmica de informações no terminal.
* Aplicação prática das Heurísticas de Nielsen.
* Importância do feedback visual para a Experiência do Usuário (UX).

---

## 👩‍💻 Autora

**Ludmilla Santos**

Estudante de Ciência da Computação
