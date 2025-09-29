 Relatório: Filas de Pacientes

 Tipos de Fila Implementadas

- Fila Normal (array simples)
- Fila Circular (array com reaproveitamento)
- Fila Encadeada (linked list)
- Fila Prioritária (com base na prioridade)
- Lista de Pacientes (lista encadeada)

## Resultados dos Testes

Todos os testes passaram com sucesso:

- Inserções e remoções realizadas corretamente
- Impressões de resultados esperados

---

## Análise de Complexidade

| Operação           | Fila Normal | Fila Circular | Fila Encadeada | Fila Prioritária |
|--------------------|-------------|---------------|----------------|------------------|
| Inserção (enqueue) | O(1)        | O(1)          | O(1)           | O(n)*            |
| Remoção (dequeue)  | O(n)*       | O(1)          | O(1)           | O(1)             |

\* Fila Normal precisa deslocar elementos ao remover → custo O(n)  
\* Fila Prioritária ordena após cada inserção → custo O(n)

---

## Conclusões

- **Mais eficiente** para inserções/remoções: **Fila Circular** e **Fila Encadeada**
- **Fila Prioritária** é útil quando há critérios de prioridade, mas tem custo maior na inserção.
- **Fila Circular** aproveita melhor o espaço do array.
- **Fila Encadeada** tem melhor escalabilidade para estruturas dinâmicas.

---

## Sugestão

Use:
- **Fila Circular** se quiser performance com uso fixo de memória.
- **Fila Encadeada** para listas de tamanho dinâmico.
- **Fila Prioritária** se prioridade entre pacientes for crítica.
