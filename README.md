# Spotify Songs Dataset

Este conjunto de dados contém informações sobre cerca de 5000 músicas provenientes da API do Spotify, coletadas usando o pacote `spotifyr`. Os dados foram utilizados por Kaylin Pavlik em um blogpost recente para explorar e classificar músicas com base em suas características de áudio. As músicas foram categorizadas em seis principais gêneros: EDM, Latino, Pop, R&B, Rap e Rock.

| Variável                  | Tipo      | Descrição                                                                                                                              |
|---------------------------|-----------|----------------------------------------------------------------------------------------------------------------------------------------|
| track_id                  | character | Identificação única da música.                                                                                                          |
| track_name                | character | Nome da música.                                                                                                                        |
| track_artist              | character | Artista da música.                                                                                                                      |
| track_popularity          | double    | Popularidade da música (0-100), onde maior é melhor.                                                                                    |
| track_album_id            | character | Identificação única do álbum.                                                                                                           |
| track_album_name          | character | Nome do álbum da música.                                                                                                                |
| track_album_release_date  | character | Data de lançamento do álbum.                                                                                                            |
| playlist_name             | character | Nome da playlist.                                                                                                                       |
| playlist_id               | character | Identificação da playlist.                                                                                                               |
| playlist_genre            | character | Gênero da playlist.                                                                                                                     |
| playlist_subgenre         | character | Subgênero da playlist.                                                                                                                  |
| danceability              | double    | Descreve o quão adequada é uma música para dançar com base em uma combinação de elementos musicais, incluindo ritmo, batida e regularidade geral. Um valor de 0.0 é o menos dançante e 1.0 é o mais dançante. |
| energy                    | double    | Medida de intensidade e atividade de uma música em uma escala de 0.0 a 1.0.                                                             |
| key                       | double    | Estimativa da tonalidade geral da música. Inteiros mapeiam notas usando notação padrão de classes de tonalidade. Por exemplo, 0 = C, 1 = C♯/D♭, 2 = D, e assim por diante. Se nenhuma tonalidade for detectada, o valor é -1. |
| loudness                  | double    | Volume geral de uma música em decibéis (dB). Valores típicos variam entre -60 e 0 dB.                                                 |
| mode                      | double    | Indica a modalidade (maior ou menor) de uma música, o tipo de escala a partir da qual seu conteúdo melódico é derivado.                |
| speechiness               | double    | Detecta a presença de palavras faladas em uma música. Valores acima de 0.66 descrevem faixas que provavelmente são feitas inteiramente de palavras faladas. Valores abaixo de 0.33 provavelmente representam músicas e outros tipos de faixas não faladas. |
| acousticness              | double    | Medida de confiança de 0.0 a 1.0 se a música é acústica. 1.0 representa alta confiança de que a música é acústica.                   |
| instrumentalness          | double    | Prevê se uma música contém ou não vocais. Valores acima de 0.5 são destinados a representar faixas instrumentais.                      |
| liveness                  | double    | Detecta a presença de uma plateia na gravação de uma música. Valores acima de 0.8 indicam alta probabilidade de a música ser ao vivo. |
| valence                   | double    | Medida de positividade musical de uma faixa em uma escala de 0.0 a 1.0.                                                                |
| tempo                     | double    | Estimativa geral do tempo de uma música em batidas por minuto (BPM).                                                                    |


Os dados estão disponíveis no arquivo `spotify_songs.csv` e consistem nos seguintes campos:

## Dicionário de Dados

- **track_id:** ID único da música no Spotify.
- **track_name:** Nome da música.
- **track_artist:** Artista da música.
- **track_popularity:** Popularidade da música numa escala de 0 a 100, indicando sua aceitação e popularidade.
- **track_album_id:** ID único do álbum ao qual a música pertence.
- **track_album_name:** Nome do álbum que contém a música.
- **track_album_release_date:** Data de lançamento do álbum.
- **playlist_name:** Nome da playlist à qual a música está associada.
- **playlist_id:** ID da playlist.
- **playlist_genre:** Gênero da playlist.
- **playlist_subgenre:** Subgênero da playlist.

### Características de Áudio

- **danceability:** Descreve a adequação da música para dançar numa escala de 0.0 a 1.0.
- **energy:** Medida de intensidade e atividade da música, variando de 0.0 a 1.0.
- **key:** Estimativa da chave musical da faixa, usando notação de Classe de Altura.
- **loudness:** Volume geral da música em decibéis (dB).
- **mode:** Indica se a música é maior (1) ou menor (0) em termos de escala musical.
- **speechiness:** Detecta a presença de palavras faladas numa faixa, variando de 0.0 a 1.0.
- **acousticness:** Medida de confiança de 0.0 a 1.0 de se a faixa é acústica.
- **instrumentalness:** Prevê se a faixa contém ou não vocais, variando de 0.0 a 1.0.
- **liveness:** Detecta a presença de audiência numa gravação ao vivo.
- **valence:** Medida de positividade musical numa escala de 0.0 a 1.0.
- **tempo:** Estimativa do tempo da música em batidas por minuto (BPM).
- **duration_ms:** Duração da música em milissegundos.

## Fonte dos Dados
Os dados foram obtidos através do pacote `spotifyr`, criado por Charlie Thompson, Josiah Parry, Donal Phipps e Tom Wolff. Agradecimentos especiais a Kaylin Pavlik pelo uso desses dados em sua análise, bem como a Jon Harmon e Neal Grantham.

Para acessar os dados, utilize o seguinte link: [Spotify Songs Dataset](https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2020/2020-01-21/spotify_songs.csv)

## Referências e Pacotes Relacionados
- [Pacote spotifyr](https://github.com/charlie86/spotifyr)
- [Post de Kaylin Pavlik utilizando características de áudio](link_para_o_post_aqui)
- [Pacote tidytuesdayR](https://github.com/thebioengineer/tidytuesdayR)

---

Este README fornece uma visão geral do conjunto de dados, incluindo sua fonte, significado dos campos e links para a obtenção dos dados originais e referências relevantes.