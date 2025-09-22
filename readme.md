# 📦 Sistema de Cadastro de Estoque

Um sistema web simples e intuitivo para controle de estoque, desenvolvido com HTML, CSS e JavaScript vanilla.

## ✨ Funcionalidades

- 📊 **Saldo Inicial**: Define o estoque inicial do sistema
- ➕ **Entradas**: Registra produtos adicionados ao estoque
- ➖ **Saídas**: Registra produtos retirados do estoque (com validação de saldo)
- 🔍 **Validações**: 
  - Verificação de tipos de operação válidos (1 ou 2)
  - Validação de quantidades positivas
  - Controle de saldo insuficiente
- 📱 **Interface Visual**: Feedback colorido para diferentes tipos de operações
- 🔄 **Loop Contínuo**: Sistema roda até o usuário escolher encerrar

## 🎨 Interface

O sistema utiliza um design clean com código de cores:
- 🟢 **Verde**: Entradas no estoque
- 🔴 **Vermelho**: Saídas do estoque e erros
- 🟡 **Amarelo**: Exibição do saldo atual
- 🔵 **Azul**: Mensagem de sistema encerrado

## 🚀 Como Usar

1. **Abra o arquivo `estoque.html` em seu navegador**
2. **Digite o saldo inicial** quando solicitado
3. **Para cada operação:**
   - Escolha o tipo: `1` para Entrada ou `2` para Saída
   - Informe a quantidade desejada
   - O sistema calculará automaticamente o novo saldo
4. **Continue** operando ou digite `S` para encerrar

## 📋 Fluxo do Sistema

```
Início → Saldo Inicial → Loop Principal
  ↓
Tipo de Operação (1-Entrada / 2-Saída)
  ↓
Validação de Tipo
  ↓
Quantidade
  ↓
Validação de Quantidade
  ↓
Processamento (Entrada/Saída)
  ↓
Exibir Saldo Atual
  ↓
Continuar? (S/N) → Se N, volta ao Loop
  ↓
Sistema Encerrado + Saldo Final
```
![Fluxograma](/Fluxograma-Logica-Estoque-Senai.png)

## 💻 Tecnologias Utilizadas

- ![HTML5](https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) **HTML5**: Estrutura da página
- ![CSS3](https://img.shields.io/badge/-CSS3-1572B6?style=flat-square&logo=css3&logoColor=white) **CSS3**: Estilização e layout responsivo
- ![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) **JavaScript**: Lógica de negócio e interatividade

## 🔧 Recursos Técnicos

### Variáveis e Escopo
- `const`: Para mensagens fixas que não mudam
- `let`: Para variáveis que sofrem alterações (saldo, tipo, quantidade)

### Estruturas de Controle
- `while`: Loop principal do sistema
- `do...while`: Validação de entrada de dados
- `if...else`: Condicionais para tipos de operação

### Validações Implementadas
- `parseInt()`: Conversão de strings para números
- `isNaN()`: Verificação de valores numéricos válidos
- `toUpperCase()`: Padronização de entrada S/N

## 📝 Exemplo de Uso

```
Saldo inicial: 100

Operação: Entrada de 50 unidades
→ Saldo atual: 150

Operação: Saída de 30 unidades  
→ Saldo atual: 120

Operação: Saída de 200 unidades
→ ❌ Saldo insuficiente
→ Saldo atual: 120

Sistema Encerrado!
Saldo final: 120
```

## 🎯 Características

- ✅ **Simples e Funcional**: Interface minimalista e fácil de usar
- ✅ **Validação Robusta**: Impede operações inválidas
- ✅ **Feedback Visual**: Cores diferentes para cada tipo de operação
- ✅ **Controle de Fluxo**: Loop contínuo até encerramento manual
- ✅ **Responsivo**: Funciona em qualquer navegador moderno

## 📦 Como Executar

1. Faça o download do arquivo `estoque.html`
2. Abra o arquivo em qualquer navegador web moderno
3. Siga as instruções na tela 

---

Desenvolvido com ❤️ para controle simples e eficiente de estoque!
