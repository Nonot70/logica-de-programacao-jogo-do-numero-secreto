# 🎮 Lógica de Programação com JavaScript  
**Curso:** Lógica de Programação: mergulhe em programação com JavaScript – Alura   

---

## 📘 Sobre o curso  

Este repositório reúne todo o aprendizado adquirido no curso **“Lógica de Programação: mergulhe em programação com JavaScript”**, onde desenvolvi um projeto prático — o **Jogo do Número Secreto** — aplicando fundamentos essenciais da programação e boas práticas de código.

Durante as aulas, aprendi a estruturar o raciocínio lógico para resolver problemas, dominar conceitos fundamentais de variáveis, loops e condicionais, e compreender como o JavaScript se comunica com o navegador.

---

## 🚀 Principais aprendizados  

### 🧠 Lógica de Programação
- Entendimento de **algoritmos**: passo a passo para resolver problemas com clareza.  
- Uso de **comentários** (`//`) e organização do raciocínio lógico no código.  
- Criação de **estruturas condicionais** (`if`, `else`) para decisões automáticas.  
- Aplicação de **loops** (`while`) para repetição de ações até atingir um objetivo.  
- Manipulação de **variáveis** com `let` e exibição de mensagens com `alert` e `prompt`.

### 💬 Interatividade e feedback
- Implementação de respostas dinâmicas no jogo (maior/menor, acerto, erro).  
- Exibição de mensagens e contagem de tentativas do jogador.  
- Criação de mensagens personalizadas no singular ou plural com o **operador ternário**.

### 🎲 Aleatoriedade e funções matemáticas
- Utilização de `Math.random()` e `parseInt()` para gerar números aleatórios.  
- Definição de intervalos dinâmicos e variáveis configuráveis (`numeroMaximo`).  
- Entendimento do conceito de **número pseudoaleatório** e arredondamento.

### ⚙️ Boas práticas de desenvolvimento
- Padronização do uso de aspas simples e ponto e vírgula.  
- Nomeação clara e semântica de variáveis (`numeroSecreto`, `tentativas`, `chute`).  
- Indentação e legibilidade do código.  
- Uso da extensão **Live Server** para atualização automática no navegador.

---

## 💻 Tecnologias utilizadas  

| Tecnologia | Finalidade |
|-------------|-------------|
| **JavaScript (ES6+)** | Lógica do jogo e interação com o usuário |
| **HTML5** | Estrutura da página |
| **CSS3** | Estilização visual |
| **Visual Studio Code** | Ambiente de desenvolvimento |
| **Live Server** | Atualização automática do projeto |

---

## 🧩 Projeto desenvolvido: *Jogo do Número Secreto*  

Um jogo simples e divertido que desafia o usuário a adivinhar o número gerado pelo computador.  
O sistema informa se o palpite é **maior ou menor** e contabiliza quantas tentativas foram necessárias até o acerto.

```javascript
let numeroMaximo = 100;
let numeroSecreto = parseInt(Math.random() * numeroMaximo + 1);
let chute;
let tentativas = 1;

while (chute != numeroSecreto) {
  chute = prompt(`Escolha um número entre 1 e ${numeroMaximo}`);

  if (chute == numeroSecreto) {
    let palavraTentativa = tentativas > 1 ? 'tentativas' : 'tentativa';
    alert(`Isso aí! Você descobriu o número secreto ${numeroSecreto} com ${tentativas} ${palavraTentativa}.`);
  } else {
    if (chute > numeroSecreto) {
      alert(`O número secreto é menor que ${chute}`);
    } else {
      alert(`O número secreto é maior que ${chute}`);
    }
    tentativas++;
  }
}
```
---

## 🎯 Desafios superados  

- Compreender a diferença entre **atribuição (`=`)** e **comparação (`==`)**.  
- Implementar **loops** sem criar loops infinitos.  
- Garantir a **concordância gramatical** nas mensagens de saída.  
- Criar **variáveis dinâmicas** para alterar o intervalo de números do jogo.  
- Aplicar **boas práticas de refatoração**, tornando o código mais limpo e legível.  

---

## 🧭 Conceitos complementares  

- **Operadores lógicos:** `&&`, `||`, `!`  
- **Controle de fluxo:** `if`, `else`, `while`, `break`  
- **Template Strings:** uso de crases (`` ` ``) e variáveis dinâmicas `${}`  
- **Operador ternário:** simplificação de condições (`condição ? A : B`)  
- **Depuração:** uso de `console.log()` para testar valores e validar lógicas.  

---

## 🏆 Conclusão  

Esse projeto marcou o início da minha jornada no desenvolvimento com **JavaScript**.  
Com ele, aprendi que programar vai além de escrever código — é **raciocinar, testar, errar e melhorar** a cada tentativa.  

> 💬 “Programar é transformar ideias em lógica, passo a passo, até virar realidade.”  

Este curso me deu uma **base sólida** para seguir aprendendo novas linguagens, frameworks e conceitos mais avançados em **desenvolvimento web**.
