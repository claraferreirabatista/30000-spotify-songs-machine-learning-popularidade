# Spotify Songs Dataset

Este conjunto de dados contém informações sobre cerca de 5000 músicas provenientes da API do Spotify, coletadas usando o pacote `spotifyr`. Os dados foram utilizados por Kaylin Pavlik em um blogpost recente para explorar e classificar músicas com base em suas características de áudio. As músicas foram categorizadas em seis principais gêneros: EDM, Latino, Pop, R&B, Rap e Rock.

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