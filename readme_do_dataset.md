

![@neonbrand via Unsplash - pessoa segurando iPhone 6 cinza espacial](https://images.unsplash.com/photo-1495434942214-9b525bba74e9?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80)

# Músicas no Spotify

Os dados desta semana vêm do Spotify por meio do pacote [`spotifyr`](https://www.rcharlie.com/spotifyr/). [Charlie Thompson](https://twitter.com/_RCharlie), [Josiah Parry](https://twitter.com/JosiahParry), Donal Phipps e Tom Wolff desenvolveram este pacote para facilitar a obtenção de seus próprios dados ou metadados gerais sobre músicas da API do Spotify. Certifique-se de verificar o site do pacote [`spotifyr`](https://www.rcharlie.com/spotifyr/) para ver como você pode coletar seus próprios dados!

[Kaylin Pavlik](https://twitter.com/kaylinquest/status/1213138536570015745) fez recentemente uma [postagem no blog](https://www.kaylinpavlik.com/classifying-songs-genres/) usando as características de áudio para explorar e classificar músicas. Ela usou o pacote `spotifyr` para coletar cerca de 5000 músicas de 6 categorias principais (EDM, Latin, Pop, R&B, Rap e Rock).

Créditos a [Jon Harmon](https://github.com/rfordatascience/tidytuesday/issues/160) e [Neal Grantham](https://twitter.com/nsgrantham/status/1213190975113199616).

### Obtenha os dados aqui

```{r}
# Obter os Dados

spotify_songs <- readr::read_csv('https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2020/2020-01-21/spotify_songs.csv')

# Ou leia com o pacote tidytuesdayR (https://github.com/thebioengineer/tidytuesdayR)
# ATENÇÃO: PARA USAR OS DADOS DE 2020, VOCÊ PRECISA ATUALIZAR O tidytuesdayR no GitHub

# Você pode instalar via devtools::install_github("thebioengineer/tidytuesdayR")

tuesdata <- tidytuesdayR::tt_load('2020-01-21') 
tuesdata <- tidytuesdayR::tt_load(2020, week = 4)

spotify_songs <- tuesdata$spotify_songs
```

### Dicionário de Dados

# `spotify_songs.csv`

|variável                 |classe     |descrição |
|:---|:---|:-----------|
|track_id                 |character | ID único da música|
|track_name               |character | Nome da música|
|track_artist             |character | Artista da música|
|track_popularity         |double    | Popularidade da música (0-100) onde valores mais altos são melhores |
|track_album_id           |character | ID único do álbum|
|track_album_name         |character | Nome do álbum da música |
|track_album_release_date |character | Data de lançamento do álbum |
|playlist_name            |character | Nome da playlist |
|playlist_id              |character | ID da playlist|
|playlist_genre           |character | Gênero da playlist |
|playlist_subgenre        |character | Subgênero da playlist|
|danceability             |double    | A dançabilidade descreve o quão adequada uma faixa é para dançar com base em uma combinação de elementos musicais, incluindo tempo, estabilidade rítmica, força do ritmo e regularidade geral. Um valor de 0,0 é o menos dançável e 1,0 é o mais dançável. |
|energy                   |double    | Energia é uma medida de 0,0 a 1,0 que representa uma medida perceptual de intensidade e atividade. Tipicamente, faixas energéticas parecem rápidas, altas e barulhentas. Por exemplo, o death metal tem alta energia, enquanto um prelúdio de Bach pontua baixo na escala. As características perceptuais que contribuem para este atributo incluem faixa dinâmica, volume percebido, timbre, taxa de início e entropia geral. |
|key                      |double    | A chave geral estimada da faixa. Os inteiros mapeiam para tons usando a notação padrão de Classe de Tons. Por exemplo, 0 = C, 1 = C♯/Ré♭, 2 = D, e assim por diante. Se nenhuma chave foi detectada, o valor é -1. |
|loudness                 |double    | O volume geral de uma faixa em decibéis (dB). Os valores de volume são calculados em toda a faixa e são úteis para comparar o volume relativo das faixas. O volume é a qualidade de um som que é o correlato psicológico primário da força física (amplitude). Os valores geralmente variam entre -60 e 0 dB.|
|mode                     |double    | O modo indica a modalidade (maior ou menor) de uma faixa, o tipo de escala a partir da qual seu conteúdo melódico é derivado. Maior é representado por 1 e menor é 0.|
|speechiness              |double    | Speechiness detecta a presença de palavras faladas em uma faixa. Quanto mais exclusivamente a gravação se assemelha a fala (por exemplo, programa de entrevistas, audiolivro, poesia), mais próximo de 1,0 é o valor do atributo. Valores acima de 0,66 descrevem faixas que provavelmente consistem inteiramente de palavras faladas. Valores entre 0,33 e 0,66 descrevem faixas que podem conter música e fala, seja em seções ou sobrepostas, incluindo casos como música rap. Valores abaixo de 0,33 provavelmente representam música e outras faixas não relacionadas a fala. |
|acousticness             |double    | Uma medida de confiança de 0,0 a 1,0 de se a faixa é acústica. 1,0 representa alta confiança de que a faixa é acústica.|
|instrumentalness         |double    | Prevê se uma faixa não contém vocais. Sons como "ooh" e "aah" são tratados como instrumentais nesse contexto. Faixas