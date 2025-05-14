# Algoritmos Genéticos

### Algoritmos evolucionários e algoritmos genéticos

**Algoritmos evolucionários (EA - evolutionary algorithm)**
- Modelos computacionais dos processos naturais de evolução.
- Simulação da evolução das espécies.
- Sobrevivência do mais apto.
- Auto organização, comportamento adaptativo.

**Algoritmos genéticos**
- Ramos dos algoritmos evolucionários.
- Soluções cada vez melhores a partir da evolução das gerações anteriores.
- Redes neurais.
- - Os algoritmos genéticos são muito utilizados em combinação com redes neurais artificiais.
- - O algoritmo *back-propagation*, que existe para encontrar os melhores pesos de uma rede neural utilizam conceitos de algoritmos genéticos.
- Não somente são usados para resolver problemas do mundo real, mas também para auxiliar outros algoritmos de Machine Learning.

#### Fluxo de um algoritmo genético:

![fluxo ag](readme_imgs/image.png)

## Características dos algoritmos genéticos

### Indivíduo
- Indivíduos representam as soluções.
- Cada indivíduo vai representar uma solução específica para o problema e cabe a nós definir qual deles representa a melhor solução.
- **Um conjunto de indivíduos formam uma população**.
- O **cromossomo representa uma solução para o problema**.
- O indivíduo pode ser o próprio cromossomo na maneira mais simples possível, ou pode conter o cromossomo como atributo.

Exemplo, para os objetos Celular, Caderno, Livro e Notebook é necessário colocar em uma mochila de tamanho X estes objetos, porém a mochila não cabe todos. Assim como, vamos supor que seja necessário ter os objetosmais caros nessa mochila, então quais objetos seriam podem ser escolhidos, que sejam os mais caros e que caibam na mochila?

```py
    cromossomo = [
        ['Celular', 0],
        ['Caderno', 1],
        ['Livro', 0],
        ['Notebook', 1]
    ]
```

Um cromossomo nada mais é do que um conjunto de respostas, onde nesse contexto há valores 0 ou 1 para alguns objetos que podem significar uma solução de objetos que serão levados e os que não serão levados.

Ou seja, cada indivíduo da população é uma possível resposta para o problema sendo resolvido, geralmente representado por um cromossomo, que codifica os parâmetros ou variáveis da solução.

**Cada indivíduo da população é composto por um único cromossomo, ou seja, um indivíduo é uma solução, e seu cromossomo é a forma como essa solução está representada internamente.** Durante o processo evolutivo, os cromossomos são cruzados e modificados, originando, assim, novos indivíduos que compõem a próxima geração.