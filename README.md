# wordbombdb-pt

Lista de **20.000 palavras em português (pt-BR)**, ordenadas por frequência de uso — da mais comum para a menos comum. Uma palavra por linha, tudo em minúsculas, formato UTF-8.

Criada para jogos de palavras (como Word Bomb), no mesmo formato do [wordbombdb](https://github.com/its-jonas/wordbombdb) em inglês.

## Arquivo

- [`20k.txt`](20k.txt) — 20.000 palavras, uma por linha

## Como foi gerada

1. Base de frequência: lista pt_BR do [FrequencyWords](https://github.com/hermitdave/FrequencyWords) (corpus OpenSubtitles 2018)
2. Filtro: apenas palavras com 2+ letras contendo somente letras do alfabeto português (a–z, á à â ã é ê í ó ô õ ú ç ü)
3. Validação: cada palavra foi cruzada com dicionários de português (lista br.ispell do IME-USP + [pythonprobr/palavras](https://github.com/pythonprobr/palavras)) para remover nomes próprios, erros e palavras estrangeiras
4. Corte nas 20.000 palavras mais frequentes, mantendo a ordem por frequência
