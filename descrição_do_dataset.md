### Descrição do Dataset

#### Shape Atual do Dataset:
- Após a limpeza de dados, o dataset agora possui dimensões (9864, 16).

#### Colunas Restantes:
1. **track_popularity:**
   - Descrição: Indica a popularidade da música em uma escala de 0 a 100, onde valores mais altos indicam maior popularidade.

2. **playlist_genre:**
   - Descrição: Gênero da playlist à qual a música pertence.

3. **playlist_subgenre:**
   - Descrição: Subgênero da playlist.

4. **danceability:**
   - Descrição: Medida que descreve o quão adequada é uma música para dançar, baseada em elementos como ritmo e batida.

5. **energy:**
   - Descrição: Medida de intensidade e atividade de uma música em uma escala de 0.0 a 1.0.

6. **key:**
   - Descrição: Estimativa da tonalidade geral da música, representada por inteiros mapeados usando notação padrão de classes de tonalidade.

7. **loudness:**
   - Descrição: Volume geral de uma música em decibéis (dB).

8. **mode:**
   - Descrição: Indica a modalidade (maior ou menor) de uma música.

9. **speechiness:**
   - Descrição: Detecta a presença de palavras faladas em uma música.

10. **acousticness:**
    - Descrição: Medida de confiança de 0.0 a 1.0 se a música é acústica.

11. **instrumentalness:**
    - Descrição: Prevê se uma música contém ou não vocais.

12. **liveness:**
    - Descrição: Detecta a presença de uma plateia na gravação de uma música.

13. **valence:**
    - Descrição: Medida de positividade musical de uma faixa em uma escala de 0.0 a 1.0.

14. **tempo:**
    - Descrição: Estimativa geral do tempo de uma música em batidas por minuto (BPM).

15. **duration_ms:**
    - Descrição: Duração da música em milissegundos.

16. **popularity_class:**
    - Descrição: Classe de popularidade atribuída à música (0, 1, 2 ou 3).


#### Média da Popularidade por Classe:
- Classe 0: 11.97
- Classe 1: 32.61
- Classe 2: 50.32
- Classe 3: 74.27

#### Correlações entre Features Numéricas e 'track_popularity':

- **danceability:** 0.166
- **energy:** -0.145
- **key:** 0.036
- **loudness:** 0.107
- **mode:** -0.005
- **speechiness:** 0.099
- **acousticness:** 0.088
- **instrumentalness:** -0.216
- **liveness:** -0.068
- **valence:** 0.138
- **tempo:** -0.034

## Features numéricas com suas estatísticas:

#### track_popularity

| Estatística       | Valor   |
|-------------------|---------|
| Média             | 51.01   |
| Desvio Padrão     | 20.83   |
| Mínimo            | 0       |
| 25%               | 37      |
| 50%               | 50      |
| 75%               | 66      |
| Máximo            | 100     |

#### danceability

| Estatística       | Valor   |
|-------------------|---------|
| Média             | 0.677   |
| Desvio Padrão     | 0.136   |
| Mínimo            | 0.077   |
| 25%               | 0.592   |
| 50%               | 0.691   |
| 75%               | 0.775   |
| Máximo            | 0.979   |

#### energy

| Estatística       | Valor   |
|-------------------|---------|
| Média             | 0.695   |
| Desvio Padrão     | 0.178   |
| Mínimo            | 0.0167  |
| 25%               | 0.58    |
| 50%               | 0.712   |
| 75%               | 0.831   |
| Máximo            | 1       |

#### key

| Estatística       | Valor   |
|-------------------|---------|
| Média             | 5.38    |
| Desvio Padrão     | 3.64    |
| Mínimo            | 0       |
| 25%               | 2       |
| 50%               | 6       |
| 75%               | 9       |
| Máximo            | 11      |

#### loudness

| Estatística       | Valor    |
|-------------------|----------|
| Média             | -6.33    |
| Desvio Padrão     | 2.76     |
| Mínimo            | -26.207  |
| 25%               | -7.614   |
| 50%               | -5.8585  |
| 75%               | -4.458   |
| Máximo            | 0.326    |

#### mode

| Estatística       | Valor   |
|-------------------|---------|
| Média             | 0.54    |
| Desvio Padrão     | 0.50    |
| Mínimo            | 0       |
| 25%               | 0       |
| 50%               | 1       |
| 75%               | 1       |
| Máximo            | 1       |

#### speechiness

| Estatística       | Valor   |
|-------------------|---------|
| Média             | 0.114   |
| Desvio Padrão     | 0.101   |
| Mínimo            | 0.023   |
| 25%               | 0.045   |
| 50%               | 0.072   |
| 75%               | 0.146   |
| Máximo            | 0.877   |

#### acousticness

| Estatística       | Valor   |
|-------------------|---------|
| Média             | 0.191   |
| Desvio Padrão     | 0.225   |
| Mínimo            | 0.000001|
| 25%               | 0.0189  |
| 50%               | 0.101   |
| 75%               | 0.288   |
| Máximo            | 0.986   |

#### instrumentalness

| Estatística       | Valor   |
|-------------------|---------|
| Média             | 0.095   |
| Desvio Padrão     | 0.239   |
| Mínimo            | 0       |
| 25%               | 0       |
| 50%               | 0.000009|
| 75%               | 0.00432 |
| Máximo            | 0.994   |

#### liveness

| Estatística       | Valor   |
|-------------------|---------|
| Média             | 0.185   |
| Desvio Padrão     | 0.147   |
| Mínimo            | 0.0131  |
| 25%               | 0.0953  |
| 50%               | 0.125   |
| 75%               | 0.231   |
| Máximo            | 0.979   |

#### valence

| Estatística       | Valor   |
|-------------------|---------|
| Média             | 0.481   |
| Desvio Padrão     | 0.226   |
| Mínimo            | 0.00001 |
| 25%               | 0.307   |
| 50%               | 0.478   |
| 75%               | 0.654   |
| Máximo            | 0.981   |

#### tempo

| Estatística       | Valor    |
|-------------------|----------|
| Média             | 122.28   |
| Desvio Padrão     | 26.69    |
| Mínimo            | 35.48    |
| 25%               | 100.38   |
| 50%               | 123.95   |
| 75%               | 135.82   |
| Máximo            | 219.99   |

#### duration_ms

| Estatística       | Valor      |
|-------------------|------------|
| Média             | 197699.04  |
| Desvio Padrão     | 44754.76   |
| Mínimo            | 54656      |
| 25%               | 170057.5   |
| 50%               | 192839     |
| 75%               | 218182     |
| Máximo            | 515703     |

#### popularity_class

| Estatística       | Valor   |
|-------------------|---------|
| Média             | 1.93    |
| Desvio Padrão     | 0.94    |
| Mínimo            | 0       |
| 25%               | 1       |
| 50%               | 2       |
| 75%               | 3       |
| Máximo            | 3       |

