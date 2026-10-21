# Aula Prática: Algoritmos de Programação

**Instituição:** PUC Goiás  
**Curso:** EAD - Análise e Desenvolvimento de Sistemas (ADS) e Big Data  
**Duração:** 40 minutos  
**Formato:** Aula Online Prática  

---

## Objetivos da Aula
- Compreender o conceito fundamental de algoritmo e sua aplicação no cotidiano.
- Entender a função das variáveis e os tipos de dados.
- Estruturar um pseudocódigo de forma correta e sequencial.
- Representar algoritmos graficamente através de fluxogramas (ferramenta: draw.io).
- Analisar e corrigir falhas lógicas em fluxogramas.

---

## Bloco 1: Fundamentos e a Lógica do Cotidiano (10 min)

### O que é um algoritmo?
Uma sequência finita de operações que, quando executadas na ordem estabelecida, atingem um objetivo determinado em um tempo finito. Um algoritmo correto possui:
* Estado inicial;
* Ações claras e precisas;
* Saídas corretas;
* Estado final previsível.

### O Tripé Computacional
Todo programa baseia-se em três etapas essenciais:
1. **Entrada:** Obtenção de dados.
2. **Processamento:** Cálculos e manipulação de informações.
3. **Saída:** Exibição dos resultados.

### Exemplo Prático: Eficiência na Cozinha (Ovo Mexido)
* **Eficácia vs. Eficiência:** Um algoritmo pode funcionar (ser eficaz), mas gastar recursos desnecessários (ineficiente).
* **Cenário:** Instruir o usuário a ligar o fogão no passo 1, antes mesmo de separar os ingredientes, quebrar o ovo e bater com sal. O ovo será feito, mas haverá desperdício de gás.
* **Solução:** Reordenar o passo de "ligar o fogão" para o momento exato antes de colocar a manteiga na frigideira, otimizando o algoritmo.

---

## Bloco 2: Variáveis e Estrutura do Pseudocódigo (15 min)

### O Papel das Variáveis e Tipagem
Variáveis são espaços reservados na memória principal (RAM) para guardar valores durante o processamento. Cada variável armazena um valor por vez e possui um tipo específico:
* `inteiro`: Valores numéricos sem casas decimais.
* `real`: Valores numéricos fracionários.
* `caractere`: Apenas uma letra, número ou símbolo.
* `string`: Cadeia de texto (ex: "Ana Maria").
* `lógico`: Verdadeiro ou falso.

### Estrutura Rigorosa de um Pseudocódigo
A construção deve seguir um padrão para facilitar a conversão para linguagens como C ou Pascal:
1. **Cabeçalho:** Nome do algoritmo e comentário indicando o objetivo.
2. **Declarações:** Separação clara entre `Entradas`, `Saídas` e `Variáveis auxiliares`.
3. **Corpo do Algoritmo:** Delimitado por `início` e `fim`. Cada comando deve ocupar uma linha.
4. **Comentários:** Utilização de chaves `{ }` para documentar os passos.

### Exemplo Prático 1: Cálculo de Média de Três Notas
*Apresentação da estrutura completa em pseudolinguagem.*

```text
Algoritmo CalculoMedia
{RECEBE 3 NOTAS, INFORMA AS NOTAS LIDOS, A SOMA E A MEDIA}

Entradas: nota1, nota2, nota3 (real)
Saídas: soma, media (real)

início
  ler (nota1, nota2, nota3)       {OBTÉM AS 3 NOTAS}
  escrever (nota1, nota2, nota3)  {EXIBE AS NOTAS PARA VERIFICAÇÃO}
  
  soma <- nota1 + nota2 + nota3   {CALCULA A SOMA TOTAL}
  escrever (soma)                 {INFORMA A SOMA}
  
  media <- soma / 3               {CALCULA A MÉDIA ARITMÉTICA}
  escrever (media)                {INFORMA A MÉDIA FINAL}
fim
```

---

## Bloco 3: Modelagem Visual com Fluxogramas (10 min)

### O que é um Fluxograma?
É a representação gráfica do algoritmo. Organiza as instruções visualmente para validar a lógica antes de programar.

### Simbologia Padrão
* **Elipse:** Início e Fim.
* **Paralelogramo:** Entrada e Saída de dados (ler/escrever).
* **Retângulo:** Processamento (cálculos, atribuições).
* **Setas:** Linhas de fluxo que determinam a ordem de execução.

### Exemplo Prático 2: O Fluxograma da Média (Conversão)
Mostrar como o pseudocódigo anterior se transforma em blocos:
1. `Elipse`: Início
2. `Paralelogramo`: ENTRADA nota1, nota2, nota3
3. `Paralelogramo`: SAÍDA nota1, nota2, nota3
4. `Retângulo`: soma <- nota1 + nota2 + nota3
5. `Paralelogramo`: SAÍDA soma
6. `Retângulo`: média <- soma / 3
7. `Paralelogramo`: SAÍDA média
8. `Elipse`: Fim

---

## Bloco 4: Análise de Algoritmos e Resolução de Problemas (5 min)

### Análise Crítica e Falhas Comuns
Analisar um algoritmo significa interpretar a relação entre entrada, processamento e saída.
* **Falha de Sequência:** Etapas em ordem incorreta.
* **Falha de Omissão:** Faltar um passo essencial (ex: calcular a média sem ter lido a nota).
* **Falha de Redundância:** Repetições desnecessárias.

### Exemplo Prático 3: O Fluxo Incorreto (Caça ao Erro)
*Apresentar na tela (ou via draw.io) um fluxograma de vendas com erro:*
* **Erro:** Calcular o desconto (`valor * 0,10`) antes mesmo de ler o valor do produto e a quantidade.
* **Confusão Conceitual:** Definir subtotal como `total - desconto`.
* **Resolução interativa com os alunos:**
  1. Primeiro, ler *todas* as entradas (nome, quantidade, valor do produto).
  2. Processar o subtotal (`valor do produto * quantidade`).
  3. Processar o desconto (`subtotal * 0,10`).
  4. Processar o total final (`subtotal - desconto`).
  5. Exibir os resultados.

---
**Recursos e Ferramentas:**
* Apresentação de slides para os conceitos teóricos.
* Ferramenta web **draw.io** para modelagem colaborativa/demonstração no Bloco 3 e 4.
