# 🌧️ Análise da Precipitação no Lubango, Angola (2015–2025)

## 📌 Sobre o projecto

Este projecto analisa os padrões de precipitação no Lubango, Angola, entre 2015 e 2025, com o objectivo de identificar os meses com menor disponibilidade de chuva.

A análise procura compreender em que períodos a baixa precipitação pode representar um risco para a sementeira de sequeiro, com foco na cultura do milho.

O projecto utiliza Python para recolher, organizar, analisar e visualizar dados meteorológicos.

## 🎯 Pergunta de análise

**Em que meses do ano a baixa precipitação pode representar um risco para a sementeira de sequeiro do milho no Lubango?**

## 📍 Área de estudo

- **Localização:** Lubango, Angola
- **Latitude:** -14.92
- **Longitude:** 13.49
- **Período analisado:** 2015–2025
- **Fonte dos dados:** NASA POWER API

Os dados correspondem a um ponto de grelha meteorológica próximo das coordenadas indicadas e não a medições directas de uma estação meteorológica local.

## 🛠️ Ferramentas utilizadas

- **Python:** análise dos dados.
- **Pandas:** organização e tratamento dos dados.
- **Matplotlib:** criação de gráficos.
- **Requests:** comunicação com a API.
- **NASA POWER API:** obtenção dos dados meteorológicos.
- **Google Colab:** ambiente de desenvolvimento.

## 📊 Metodologia

O trabalho foi desenvolvido nas seguintes etapas:

1. Recolha dos dados diários de precipitação através da NASA POWER API.
2. Organização e tratamento dos dados com Pandas.
3. Agrupamento dos registos diários por mês.
4. Cálculo da precipitação mensal e das médias de cada mês do calendário.
5. Identificação dos meses com precipitação média inferior a 50 mm.
6. Contagem dos anos em que cada mês registou menos de 50 mm.
7. Criação de gráficos para facilitar a interpretação dos resultados.

O valor de 50 mm foi utilizado como um critério exploratório para identificar meses com baixa precipitação. Não representa, por si só, um limite agronómico universal para determinar se a sementeira do milho é segura.

## 📈 Resultados preliminares

A análise dos dados apresenta os seguintes resultados:

- A precipitação total média anual é de aproximadamente 612 mm.
- Março apresenta a maior precipitação média mensal, com cerca de 216,22 mm.
- A precipitação concentra-se sobretudo entre Dezembro e Abril.
- Entre Maio e Outubro, os valores calculados indicam uma precipitação muito reduzida.
- Novembro apresenta uma precipitação média de aproximadamente 39,69 mm, podendo merecer atenção no planeamento da sementeira.

Estes resultados são preliminares e devem ser interpretados após a confirmação das unidades e da agregação dos dados.

### 🌧️ Precipitação média mensal

| Mês | Precipitação média (mm) |
|---|---:|
| Janeiro | 91,73 |
| Fevereiro | 126,43 |
| Março | 216,22 |
| Abril | 63,65 |
| Maio | 2,63 |
| Junho | 0,14 |
| Julho | 0,02 |
| Agosto | 0,36 |
| Setembro | 1,56 |
| Outubro | 10,90 |
| Novembro | 39,69 |
| Dezembro | 58,63 |

### 📉 Visualização dos resultados

![Precipitação média mensal no Lubango](images/precipitacao_lubango.png)

O gráfico permite comparar a precipitação média entre os meses do ano e identificar os períodos com valores mais baixos.

## 🌽 Relevância para a agricultura

A precipitação é um factor importante para a agricultura de sequeiro, uma vez que a produção depende principalmente da água fornecida pela chuva.

A identificação dos meses com menor precipitação pode ajudar a orientar estudos sobre o calendário agrícola e os possíveis períodos de défice hídrico.

No entanto, a decisão sobre a época de sementeira do milho exige informação adicional, incluindo a distribuição das chuvas, a humidade do solo, o tipo de solo e as necessidades de água da cultura.

Por isso, esta análise constitui um primeiro passo para estudar a relação entre a precipitação e o risco hídrico agrícola no Lubango.

## ⚠️ Limitações

- Os dados provêm de uma grelha meteorológica e não de uma estação local.
- O estudo considera apenas um ponto geográfico.
- O período de 11 anos é limitado para tirar conclusões sobre tendências climáticas de longo prazo.
- O critério de 50 mm é exploratório e não considera directamente as necessidades de água do milho.
- Os resultados dependem da correcta interpretação das unidades e do tratamento dos dados.

## 🚀 Possíveis melhorias

- Validar os valores de precipitação e as respectivas unidades.
- Calcular o número de anos com precipitação inferior a 50 mm em cada mês.
- Analisar a variação da precipitação entre anos.
- Estudar a relação entre a chuva e as necessidades de água do milho.
- Comparar os resultados com dados de estações meteorológicas locais, caso estejam disponíveis.

## 📚 Fonte dos dados

**NASA POWER**

Os dados foram obtidos através da NASA POWER API, utilizando o parâmetro de precipitação diária corrigida `PRECTOTCORR`.

Documentação oficial:
https://power.larc.nasa.gov/

## 👨‍💻 Autor

**António Pascoal Barros Sérgio**

Engenharia Agronómica — Instituto Politécnico da Huíla.

- GitHub: https://github.com/pascoalbarros-agtech
- LinkedIn: https://www.linkedin.com/in/pascoalbarros-agtech

---

*Projecto desenvolvido para aplicar Python e análise de dados ao estudo da precipitação e dos desafios da agricultura em Angola.*
