Precipitação no Lubango, Angola (2015–2025)

Pergunta: em que meses do ano há risco de falta de água para a sementeira de sequeiro (milho)?



![Precipitação média mensal no Lubango](images/precipitacao_lubango.png)



Dados

- Fonte: NASA POWER API (https://power.larc.nasa.gov/), precipitação diária corrigida (PRECTOTCORR).
- Local: Lubango (latitude -14,92; longitude 13,49), ponto de grelha. Não são dados de uma estação meteorológica.
- Período: 2015–2025.

Método

1. Recolha dos dados diários através da API (requests).
2. Limpeza e tratamento com pandas.
3. Soma da precipitação diária por mês e média de cada mês do calendário.
4. Marcação dos meses com média inferior a 50 mm como baixa precipitação. Este limiar é um critério de trabalho: [justificação ou referência].
5. Contagem, para cada mês, dos anos em que a precipitação ficou abaixo de 50 mm.
6. Gráfico com matplotlib.

Resultados

- Precipitação total média: cerca de 612 mm por ano.
- Cerca de 91% da chuva cai entre Dezembro e Abril. Março é o mês mais chuvoso (216 mm em média).
- De Maio a Outubro a chuva é residual. Junho e Julho ficam abaixo de 0,2 mm.
- Novembro tem média de 39,7 mm e ficou abaixo de 50 mm em [X] dos 11 anos, pelo que semear cedo envolve risco.

Média mensal (mm):

- Janeiro: 91,73
- Fevereiro: 126,43
- Março: 216,22
- Abril: 63,65
- Maio: 2,63
- Junho: 0,14
- Julho: 0,02
- Agosto: 0,36
- Setembro: 1,56
- Outubro: 10,90
- Novembro: 39,69
- Dezembro: 58,63

Limitações

- Dados em grelha de resolução grosseira, não medições locais.
- Uma só localização e 11 anos de dados: não permitem concluir sobre tendências climáticas.
- O limiar de 50 mm não considera o tipo de solo nem a fase da cultura.

Como correr

Instalar as dependências com: pip install -r requirements.txt

Abrir analise_precipitacao_lubango.ipynb no Jupyter ou no Google Colab e executar todas as células.

Autor

António Pascoal Barros Sérgio, Engenharia Agronómica, Instituto Politécnico da Huíla.

GitHub: https://github.com/pascoalbarros-agtech

LinkedIn: https://www.linkedin.com/in/pascoalbarros-agtech