# APS - COMPARAÇÃO DE DESEMPENHO E ANALISE DE PERFORMANCE DE ALGORITMOS DE ORDENACAO DE DADOS

## Sobre o projeto

Este repositório reúne o desenvolvimento da **Atividade Prática
Supervisionada (APS)** do curso de Ciência da **Computação da
Universidade Paulista (UNIP)**, vinculada aos 3º e 4º semestres.

O trabalho tem como tema **a comparação de desempenho e análise de
performance de algoritmos de ordenação de dados.** A proposta é estudar
diferentes estratégias para organizar conjuntos de números, implementar
os algoritmos selecionados e observar como eles se comportam diante de
volumes distintos de dados.

Mais do que produzir uma sequência ordenada, o projeto busca compreender
o custo computacional envolvido nesse processo. Para isso, relaciona a
fundamentação teórica, como a análise de complexidade, com testes
práticos de execução.

## Objetivos

### Objetivo geral
Analisar e comparar o funcionamento e o desempenho de três algoritmos de
ordenação, considerando suas estratégias, complexidades computacionais e
comportamento durante o processamento de conjuntos de dados.

### Objetivos específicos
- Compreender os fundamentos dos algoritmos de ordenação.
- Estudar o funcionamento do Bubble Sort, Binary Insertion Sort e
  Bucket Sort.
- Implementar os algoritmos e verificar se produzem corretamente os
  dados ordenados.
- Investigar a influência do volume e da distribuição dos dados no
  desempenho.
- Comparar o tempo de execução dos algoritmos em condições
  equivalentes.
- Relacionar os resultados observados com as complexidades teóricas.
- Aplicar conceitos de Estruturas de Dados e Programação Orientada a
  Objetos na construção e organização da solução.
  
## Algoritmos estudados
O projeto aborda três algoritmos que resolvem o mesmo problema por
estratégias diferentes.

### 1. Bubble Sort
Algoritmo de ordenação por comparação que percorre repetidamente a
coleção, comparando elementos adjacentes e trocando suas posições quando
estão fora da ordem desejada.

A cada passagem, os maiores elementos tendem a se deslocar para o final
do vetor. Na implementação otimizada discutida no trabalho, uma passagem
sem trocas permite encerrar antecipadamente a execução.

**Principais conceitos:** - Comparação de elementos adjacentes. - Trocas
(swap). - Laços de repetição. - Critério de parada. - Complexidade
quadrática nos casos médio e pior.

**Complexidade abordada:** melhor caso O(n), quando a implementação
otimizada identifica que o vetor já está ordenado; caso médio e pior
caso O(n²).

## 2. Binary Insertion Sort
Variação do Insertion Sort tradicional. O algoritmo mantém uma parte do
vetor ordenada e utiliza **busca binária** para localizar a posição em
que cada novo elemento deve ser inserido.

Depois de encontrar a posição, os elementos posteriores são deslocados
para abrir espaço para a inserção. Assim, a busca pela posição exige
menos comparações, mas os deslocamentos continuam tendo custo
significativo.

**Principais conceitos:** - Insertion Sort. - Busca binária. -
Manutenção de uma região ordenada. - Deslocamento de elementos em
vetores. - Diferença entre custo de comparação e custo de movimentação.

**Complexidade abordada:** a busca pela posição de inserção é
logarítmica, mas o custo total pode permanecer O(n²) devido aos
deslocamentos dos elementos.

## 3. Bucket Sort
Algoritmo de distribuição que divide os elementos em estruturas
intermediárias chamadas buckets (baldes). Cada valor é direcionado ao
balde correspondente à sua faixa. Em seguida, os baldes são ordenados
individualmente e seus conteúdos são reunidos para formar a sequência
final.

A implementação descrita no trabalho utiliza listas encadeadas para
armazenar os elementos dos baldes e considera números positivos e
negativos.

**Principais conceitos:** - Distribuição de dados por faixas de
valores. - Baldes e estruturas auxiliares. - Listas encadeadas. -
Ordenação local. - Coleta e reconstrução do vetor. - Influência da
distribuição dos dados na eficiência.

**Complexidade abordada:** pode apresentar desempenho médio próximo de
O(n + k), sob condições favoráveis de distribuição; o pior caso pode
chegar a O(n²), dependendo da concentração dos elementos nos baldes e do
método utilizado para ordená-los.

## Comparação geral dos algoritmos
Algoritmo Estratégia principal Característica de desempenho
Bubble Sort Comparações e trocas Simples, mas tende a entre vizinhos ser custoso em conjuntos maiores.

Binary Insertion Sort Busca binária seguida Reduz comparações, mas de deslocamentos mantém custo relevante de movimentação.

Bucket Sort Distribuição em baldes Pode ser eficiente e ordenação local quando os dados estão
bem distribuídos.

As complexidades apresentadas são referências teóricas. O desempenho observado em uma execução depende também da entrada, da implementação e do ambiente computacional.

## Conteúdos e conceitos abordados
Ao longo do desenvolvimento, a APS trabalha com conceitos importantes
para a formação em Ciência da Computação:
- **Algoritmos de ordenação:** estratégias para reorganizar elementos
  em uma sequência.
- **Análise de complexidade:** avaliação do crescimento do custo
  computacional conforme o tamanho da entrada.
- **Notação Big-O:** representação assintótica da eficiência de
  algoritmos.
- **Estruturas de dados:** vetores, listas encadeadas e estruturas
  auxiliares.
- **Busca binária:** localização de posições em uma sequência
  ordenada.
- **Comparações, trocas e deslocamentos:** operações que influenciam o
  tempo de execução.
- **Complexidade espacial:** análise da memória auxiliar utilizada.
- **Estabilidade:** preservação da ordem relativa de elementos com
  chaves iguais.
- **Entrada e saída (I/O):** distinção entre leitura dos dados e
  processamento realizado pelo algoritmo.
- **Testes experimentais:** execução controlada, coleta de tempos e
  comparação de resultados.
  
## Disciplinas relacionadas
O relatório destaca principalmente a integração entre duas disciplinas
do curso:

### Estruturas de Dados
É a base técnica do projeto. Os conceitos dessa disciplina são aplicados
na manipulação de vetores, listas encadeadas e coleções de elementos,
além do estudo das estratégias de ordenação e de suas complexidades.

A disciplina permite compreender como os dados são organizados na
memória e como diferentes estruturas e operações influenciam a
eficiência de um programa.

## Programação Orientada a Objetos (POO)
Contribui para a organização e estruturação do software. O relatório
relaciona a disciplina a conceitos como:
- **Abstração:** seleção das características relevantes para
  representar e processar os dados.
- **Encapsulamento:** organização e proteção das informações
  manipuladas pelo sistema.
- **Generics e interfaces:** reutilização de métodos de ordenação para
  diferentes tipos de objetos, conforme descrito no trabalho.
- **Organização e manutenção do código:** separação de
  responsabilidades e facilitação de futuras alterações.
  
### Integração entre as disciplinas
A APS demonstra como Estruturas de Dados e Programação Orientada a
Objetos podem trabalhar em conjunto: enquanto a POO auxilia na
organização do software, as estruturas de dados e os algoritmos definem
como os elementos são armazenados, manipulados e ordenados.

## Metodologia dos experimentos
A avaliação prática foi organizada para comparar os algoritmos sob
condições equivalentes.

### Conjuntos de dados
Foram utilizados conjuntos numéricos desordenados com três tamanhos:

Cenário Quantidade de elementos

1 1.000

2 5.000

3 10.000

Os dados foram disponibilizados em arquivos de texto para serem
carregados e processados pelos programas.

### Critério de medição
A métrica central da comparação é o **tempo gasto exclusivamente na
ordenação.**

O tempo de leitura dos arquivos e de carregamento dos dados na memória
não deve ser incluído na medição. Essa separação permite avaliar o custo
da execução dos algoritmos sem misturá-lo ao tempo das operações de
entrada e saída.

### Repetições
Cada cenário foi executado sete vezes por algoritmo. A média dos tempos
obtidos foi utilizada para representar o resultado comparativo e reduzir
a influência de variações isoladas entre execuções.

### Ambiente experimental descrito no relatório
- Processador: Intel Core i5-13420H.
- Memória RAM: 8 GB.
- Armazenamento: SSD de 512 GB.
- Equipamento: notebook Acer.
  
## Resultados e análise
Segundo o relatório, os três algoritmos concluíram a ordenação dos
conjuntos avaliados em tempos inferiores a um segundo, nas condições
experimentais utilizadas.

A análise não considera esse resultado suficiente para declarar um
algoritmo universalmente superior. A interpretação deve levar em conta:

- O tamanho do conjunto de entrada.
- A distribuição e a organização inicial dos dados.
- A quantidade de comparações, trocas e deslocamentos.
- O uso de memória auxiliar.
- As características da implementação e do ambiente de execução.
  
O objetivo da comparação é relacionar o comportamento observado nos
testes com as expectativas apresentadas na análise teórica.

## Organização do trabalho acadêmico
O relatório da APS está organizado nas seguintes partes:
- **1. Introdução:** contextualização do problema, objetivos e metodologia.
- **2. Referencial teórico:** fundamentos dos algoritmos de ordenação e suas complexidades.
- **3. Desenvolvimento:** explicação e implementação dos algoritmos.
- **4. Relacionamento entre disciplinas:** aplicação conjunta de Estruturas de Dados e Programação Orientada a Objetos.
- **5. Resultados e discussão:** apresentação e comparação dos testes.
- **6. Considerações finais:** síntese dos resultados e dos conhecimentos obtidos.
- **7. Referências bibliográficas e apêndice:** fontes consultadas, códigos e registros das execuções.

## Conclusão
A APS permite observar que algoritmos diferentes podem resolver o mesmo
problema, mas apresentar custos computacionais distintos. A escolha de
uma estratégia de ordenação deve considerar as características dos
dados, o volume de informações, as operações realizadas e os recursos
disponíveis.

O desenvolvimento do trabalho também reforça a importância de unir
teoria e prática: compreender a lógica de um algoritmo é fundamental,
mas medir seu comportamento e interpretar os resultados é igualmente
importante para avaliar soluções computacionais.

## Contexto acadêmico
- **Instituição:** Universidade Paulista (UNIP).
- **Curso:** Ciência da Computação.
- **Atividade:** Atividades Práticas Supervisionadas (APS).
- **Semestres indicados no relatório:** 3º e 4º.
- **Tema:** Comparação de Desempenho e Análise de Performance de Algoritmos de Ordenação de Dados.
- **Data indicada no relatório:** 2 de novembro de 2026.
---
Este repositório tem finalidade acadêmica e educacional, documentando o estudo, a implementação e a análise comparativa dos algoritmos apresentados na APS.
