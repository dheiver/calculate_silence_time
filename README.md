# Projeto de Análise de Tempo de Espera

Este projeto analisa o tempo de espera entre interações em uma chamada telefônica.

## DataFrame

O DataFrame utilizado contém as seguintes colunas:

- `id_ligacao`: ID da ligação telefônica
- `falante`: Papel do participante da chamada (Atendente ou Cliente)
- `tempo_inicio`: Tempo de início da interação
- `tempo_fim`: Tempo de fim da interação
- `tempo_espera`: Tempo de espera entre as interações
- `percentual_espera`: Percentual de espera em relação ao tempo total de espera

## Cálculo do Tempo de Espera

O tempo de espera é calculado utilizando a função `calcular_tempo_espera` que realiza as seguintes etapas:

- Calcula o tempo de espera entre as interações
- Calcula o tempo total de espera para a mesma ligação
- Calcula o percentual de espera em relação ao tempo total de espera

## DataFrame Resultante

Aqui estão as primeiras linhas do DataFrame resultante:

```python
id_ligacao   falante        tempo_inicio           tempo_fim  tempo_espera  percentual_espera
         1 Atendente 2023-07-12 09:34:08 2023-07-12 09:43:44         -60.0           0.000000
         1   Cliente 2023-07-12 09:42:44 2023-07-12 10:00:00       -2068.0           5.263158
         1 Atendente 2023-07-12 09:25:32 2023-07-12 09:42:44        -815.0          10.526316
         1   Cliente 2023-07-12 09:29:09 2023-07-12 09:25:32         326.0          15.789474
         1 Atendente 2023-07-12 09:30:58 2023-07-12 09:29:09        1414.0          21.052632
```
## Informações Adicionais

Adicione informações adicionais sobre o projeto ou análises realizadas aqui.
