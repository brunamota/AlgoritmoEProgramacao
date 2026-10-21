# Algoritmos de Programação: Introdução, Pseudocódigo e Fluxogramas

## 1.Fundamentos e a Lógica do Cotidiano

Um algoritmo é uma sequência finita de operações que, quando executadas na ordem estabelecida, atingem um objetivo determinado em um tempo finito. Para ser válido e processável, um algoritmo deve possuir um estado inicial, ações claras e precisas, saídas corretas e um estado final previsível (ele deve sempre terminar).

Todo sistema computacional, do mais simples ao mais complexo, opera sob o princípio básico do processamento de dados. Este processo é composto por três etapas fundamentais:

- **Entrada:** Obtenção dos dados necessários para a execução da tarefa.
- **Processamento:** Realização de cálculos, comparações e tomada de decisões.
- **Saída:** Informação dos resultados finais gerados.  

### Eficácia vs. Eficiência

Um algoritmo pode funcionar (ser eficaz), mas gastar recursos desnecessários (ineficiente). Ao desenvolver uma solução, dois conceitos são cruciais:

- **Eficácia (Corretude):** O algoritmo realiza a tarefa e fornece o resultado correto para quaisquer dados de entrada.
- **Eficiência:** A melhor forma de resolver o problema, otimizando o tempo de execução e o espaço de memória.

### Exemplo Prático: Preparando um Ovo Mexido

Uma receita tradicional indica: ligar o fogão, separar os ingredientes, quebrar o ovo, misturar, colocar na frigideira. Esse algoritmo é eficaz (gera o prato desejado), mas é ineficiente, pois o fogão fica ligado gastando gás desnecessariamente durante as etapas iniciais. A reordenação lógica (preparar a mistura primeiro e ligar o fogão apenas no momento da fritura) torna o algoritmo eficiente.
* **Cenário:** Instruir o usuário a ligar o fogão no passo 1, antes mesmo de separar os ingredientes, quebrar o ovo e bater com sal. O ovo será feito, mas haverá desperdício de gás.
* **Solução:** Reordenar o passo de "ligar o fogão" para o momento exato antes de colocar a manteiga na frigideira, otimizando o algoritmo.

### Um algoritmo correto possui:
* Estado inicial;
* Ações claras e precisas;
* Saídas corretas;
* Estado final previsível.

## 2. Representação Visual: Modelagem com Fluxogramas

### O que é um Fluxograma?
O fluxograma é uma representação gráfica que mapeia a sequência de ações do algoritmo. Essa etapa visualiza claramente desvios lógicos e valida a sequência das instruções antes da codificação formal.

### Simbologia Padrão
* **Elipse (Terminal):** Indica os pontos extremos do algoritmo: o `início` e o `fim`.
* **Paralelogramo:** Usado para as interações com o usuário: leitura de dados (ENTRADA) ou exibição de resultados (SAÍDA).
* **Retângulo:** Representa uma instrução de Processamento, como uma atribuição de variável ou um cálculo matemático.
* **Setas:** Linhas de fluxo que conectam os símbolos e ditam a ordem de execução passo a passo. 

### Exemplo Prático: Fluxograma de Controle de Combustível (Gestão de Frota)

<img width="2752" height="1536" alt="Gemini_Generated_Image_srq55rsrq55rsrq5" src="https://github.com/user-attachments/assets/adee964b-ecc3-43c9-8c62-48fbce70b991" />

### Exemplo Prático 2: O Fluxograma da Média (Conversão)
Mostrar como o pseudocódigo anterior se transforma em blocos:
1. `Elipse`: Início
2. `Paralelogramo`: Ler quilometragem inicial (kmInicial)
3. `Paralelogramo`: Ler quilometragem inicial (kmInicial)
4. `Retângulo`: soma <- nota1 + nota2 + nota3
5. `Paralelogramo`: SAÍDA soma
6. `Retângulo`: média <- soma / 3
7. `Paralelogramo`: SAÍDA média
8. `Elipse`: Fim

## 3. Variáveis, Tipos de Dados e Estrutura do Pseudocódigo

### **O que são Variáveis?**
Uma variável representa um espaço reservado na memória principal do computador para guardar um valor temporário durante o processamento,  ou seja, variáveis são espaços reservados na memória RAM para guardar valores durante o **processamento**. Cada variável armazena apenas um valor por vez; ao receber um novo dado, o valor anterior é permanentemente apagado.

Os dados que preenchem essas variáveis são classificados em tipos simples:
* `inteiro`: Armazena apenas valores numéricos inteiros (ex: 10, -5).
* `real`: Armazena valores numéricos fracionários (ex: 3.14, -0.5).
* `caractere`: Armazena um único caractere alfanumérico ou símbolo.
* `string`: Armazena cadeias de texto, como palavras ou frases completas.
* `lógico`: Armazena apenas dois estados, verdadeiro ou falso.

### A Estrutura Formal de um Pseudocódigo

A pseudolinguagem padroniza a lógica de programação utilizando termos em português antes de transcrevermos o código para linguagens reais (como C, Python ou Java). A estrutura obrigatória é composta por:
1. **Cabeçalho:** Inicia com a palavra Algoritmo seguida do nome do programa e um comentário curto {entre chaves} descrevendo seu objetivo.
2. **Seção de Declarações:** Todas as variáveis devem ser declaradas antes do uso, organizadas por finalidade:
  * `Entradas`: Variáveis que receberão dados do usuário.
  * `Saídas`: Variáveis que guardarão o resultado a ser exibido.
  * `Variáveis auxiliares`: Variáveis que guardam cálculos temporários (invisíveis ao usuário final).
3. **Área de Comandos:** Todo o processamento lógico ocorre obrigatoriamente entre as palavras delimitadoras início e fim. Cada comando ocupa uma linha isolada.
4. **Comentários:** Utilização de chaves `{ }` para documentar os passos.

### Exemplo Prático: Cálculo de Média de Três Notas

```text
Algoritmo CalculoMedia
{LÊ TRÊS NOTAS, EXIBE AS NOTAS, CALCULA E INFORMA A SOMA E A MÉDIA}

Entradas: nota1, nota2, nota3 (real)
Saídas: soma, media (real)

início
  ler (nota1, nota2, nota3)       {OBTÉM AS 3 NOTAS VIA TECLADO}
  escrever (nota1, nota2, nota3)  {IMPRIME AS NOTAS NA TELA PARA VERIFICAÇÃO}
  soma <- nota1 + nota2 + nota3   {PROCESSAMENTO: CALCULA A SOMA TOTAL}
  escrever (soma)                 {IMPRIME A SOMA}
  media <- soma / 3               {PROCESSAMENTO: CALCULA A MÉDIA ARITMÉTICA}
  escrever (media)                {IMPRIME A MÉDIA FINAL}
fim
```

## 4. Análise de Algoritmos e Detecção de Falhas

A construção lógica exige coerência entre os dados lidos e os processados. Analisar um algoritmo envolve buscar erros comuns que impedem a eficácia do sistema.

* **Falha de Omissão:** Esquecer de solicitar um dado de entrada essencial antes de calcular (ex: calcular uma média escolar sem ler a última nota).
* **Falha de Sequência:** Executar cálculos com variáveis que ainda não possuem valores atribuídos.
* **Falha de Redundância:** Repetições desnecessárias.

### Estudo de Caso de Falha Lógica:
Um fluxograma de frente de caixa desenhado incorretamente apresenta o seguinte bloco de cálculo:

1. Ler nome do cliente
2. Calcular desconto = valor do produto * 0.10
3. Ler valor do produto

Neste cenário, a variável valor do produto é utilizada para cálculo na Etapa 2 antes de receber o dado do usuário na Etapa 3. O computador tentará calcular 10% em cima de uma variável vazia.

**Correção da Estrutura Lógica:**
Deve-se agrupar primeiro a coleta de todos os dados e, em seguida, os cálculos em cadeia:

1. subtotal <- valor do produto * quantidade
2. desconto <- subtotal * 0.10
3. total <- subtotal - desconto
