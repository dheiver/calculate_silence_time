# Análise de Tempo de Espera em Chamadas Telefônicas

Este projeto analisa o tempo de espera entre interações em chamadas telefônicas.

## DataFrame

O DataFrame utilizado contém as seguintes colunas:

- `id_ligacao`: ID da ligação telefônica
- `falante`: Papel do participante da chamada (Atendente ou Cliente)
- `tempo_inicio`: Tempo de início da interação
- `tempo_fim`: Tempo de fim da interação
- `tempo_espera`: Tempo de espera entre as interações (em segundos)
- `tempo_total_espera`: Tempo total de espera para a mesma ligação (em segundos)
- `percentual_espera`: Percentual de espera em relação ao tempo total de espera

## Cálculo do Tempo de Espera

O tempo de espera é calculado utilizando a função `calcular_tempo_espera` que realiza as seguintes etapas:

- Agrupa os dados por ID da ligação
- Calcula o tempo de espera entre as interações
- Calcula o tempo total de espera para a mesma ligação
- Calcula o percentual de espera em relação ao tempo total de espera

## DataFrame Resultante

Aqui estão as primeiras linhas do DataFrame resultante:

```python
id_ligacao   falante        tempo_inicio           tempo_fim  tempo_espera  tempo_total_espera  percentual_espera  sobreposicao_falantes
         1 Atendente 2023-07-12 09:38:38 2023-07-12 09:36:27         257.0             24737.0               1.04                  False
         1   Cliente 2023-07-12 09:40:44 2023-07-12 10:00:00        3347.0             24737.0              13.53                   True
         1 Atendente 2023-07-12 09:04:13 2023-07-12 09:40:44        1397.0             24737.0               5.65                   True
         1   Cliente 2023-07-12 09:17:27 2023-07-12 09:04:13        3034.0             24737.0              12.27                  False
         1 Atendente 2023-07-12 09:54:47 2023-07-12 09:17:27         794.0             24737.0               3.21                  False
```
## Informações Adicionais

Adicione informações adicionais sobre o projeto ou análises realizadas aqui.
