# 📊 Dados abertos - Concurso PRF 2026 (Polícia Rodoviária Federal)

> Fatos do concurso da PRF compilados de **fontes primárias** (Diário Oficial da União, editais e PDFs oficiais do Cebraspe/CESPE) e atualizados automaticamente: um robô do [Escuta Policial](https://escutapolicial.com.br/dados/) lê o DOU a cada ~20 minutos e este repositório é espelhado a cada varredura do Radar (5x por dia).

**🌡️ Termômetro do Edital PRF em 20/07/2026: `29/100` - em aquecimento** · fase oficial: pre-edital · [metodologia](https://escutapolicial.com.br/dados/termometro-edital-prf/)

- **Licença [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.pt-br)**: copie, republique e adapte (inclusive comercialmente), **citando "Escuta Policial" com link** para https://escutapolicial.com.br/dados/.
- Nenhum número entra sem ato oficial: célula sem fonte fica vazia - preferimos a lacuna ao chute.
- Derivados (intervalos em dias, candidatos por vaga, percentuais) são **computados por script** a partir das datas e números oficiais - nunca digitados à mão.

## Datasets

| Dataset | Download | Página (metodologia + FAQ) |
| --- | --- | --- |
| Linha do tempo real dos concursos da PRF (2013-2026) | [CSV](datasets/linha-do-tempo-concurso-prf.csv) · [JSON](datasets/linha-do-tempo-concurso-prf.json) | [escutapolicial.com.br/dados/linha-do-tempo-concurso-prf/](https://escutapolicial.com.br/dados/linha-do-tempo-concurso-prf/) |
| Concorrência e abstenção do concurso PRF (2013-2021) | [CSV](datasets/concorrencia-prf.csv) · [JSON](datasets/concorrencia-prf.json) | [escutapolicial.com.br/dados/concorrencia-prf/](https://escutapolicial.com.br/dados/concorrencia-prf/) |
| Estrutura da prova da PRF por matéria: blocos oficiais × catálogo de estudo | [CSV](datasets/peso-das-materias-prf.csv) · [JSON](datasets/peso-das-materias-prf.json) | [escutapolicial.com.br/dados/peso-das-materias-prf/](https://escutapolicial.com.br/dados/peso-das-materias-prf/) |
| Termômetro do Edital PRF - índice diário de aquecimento (0-100) | [CSV](datasets/termometro-edital-prf.csv) · [JSON](datasets/termometro-edital-prf.json) | [escutapolicial.com.br/dados/termometro-edital-prf/](https://escutapolicial.com.br/dados/termometro-edital-prf/) |
| Salário do Policial Rodoviário Federal: tabela oficial de subsídio (Lei 14.875/2024) | [CSV](datasets/salario-prf.csv) · [JSON](datasets/salario-prf.json) | [escutapolicial.com.br/dados/salario-prf/](https://escutapolicial.com.br/dados/salario-prf/) |
| TAF da PRF: índices oficiais do teste de aptidão física (edital 2021) | [CSV](datasets/taf-prf.csv) · [JSON](datasets/taf-prf.json) | [escutapolicial.com.br/dados/taf-prf/](https://escutapolicial.com.br/dados/taf-prf/) |
| Requisitos e etapas do concurso da PRF (edital 2021) | [CSV](datasets/requisitos-prf.csv) · [JSON](datasets/requisitos-prf.json) | [escutapolicial.com.br/dados/requisitos-prf/](https://escutapolicial.com.br/dados/requisitos-prf/) |
| Notas de corte do concurso PRF 2021: objetiva e final, por lista | [CSV](datasets/notas-de-corte-prf-2021.csv) · [JSON](datasets/notas-de-corte-prf-2021.json) | [escutapolicial.com.br/dados/notas-de-corte-prf-2021/](https://escutapolicial.com.br/dados/notas-de-corte-prf-2021/) |
| Quem as IAs citam para estudar para a PRF (monitor mensal) | [CSV](datasets/presenca-ia.csv) · [JSON](datasets/presenca-ia.json) | [escutapolicial.com.br/dados/presenca-ia/](https://escutapolicial.com.br/dados/presenca-ia/) |

## Linha do tempo real dos concursos da PRF (2013-2026)

Quanto tempo da autorização ao edital da PRF? Ele saiu 26 dias após a autorização em 2021 e 124 dias em 2018/19. Datas oficiais de 2013, 2018/19 e 2021.

| ciclo | banca | autorizacao_dou | edital | autorizacao_para_edital_dias | prova_objetiva | edital_para_prova_dias | inscricao_inicio | inscricao_fim | inscricao_janela_dias | vagas |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2021 | Cebraspe | 2020-12-24 | 2021-01-19 | 26 | 2021-05-09 | 110 | 2021-01-25 | 2021-02-12 | 18 | 1500 |
| 2018/19 | Cebraspe | 2018-07-27 | 2018-11-28 | 124 | 2019-02-03 | 67 | 2018-12-03 | 2018-12-18 | 15 | 500 |
| 2013 | CESPE/UnB | – | 2013-06-11 | – | 2013-08-11 | 61 | 2013-06-24 | 2013-07-08 | 14 | 1000 |


**Fontes primárias:**

- Portaria SEDGG/ME nº 25.412 (DOU 24/12/2020)
- Edital nº 1 — PRF 2021, Cebraspe: https://cdn.cebraspe.org.br/concursos/PRF_21/arquivos/ED_1_PRF_2021_ABERTURA.PDF (período de inscrição e cronograma: Anexo I)
- Demanda oficial de candidatos, Cebraspe: https://cdn.cebraspe.org.br/concursos/prf_21/arquivos/PRF_21____DEMANDA_CANDIDATOS_POR_VAGA.PDF (304.330 inscritos, 1.500 vagas)
- Presentes/ausentes na prova objetiva: resultados divulgados pelo Cebraspe/PRF (205.241 presentes, 99.089 ausentes; verificado em fontes públicas em 14/07/2026)
- Portaria MP nº 236 (DOU 27/07/2018)
- Edital de abertura PRF 2018, Cebraspe (cebraspe.org.br/concursos/prf_18)
- Demanda oficial de candidatos, Cebraspe: https://cdn.cebraspe.org.br/concursos/prf_18/arquivos/PRF_18___DEMANDA.PDF (129.152 inscritos, 500 vagas, quebra por UF)
- Edital nº 1 — DPRF 2013, CESPE/UnB (cespe.unb.br/concursos/dprf_13)
- Demanda oficial de candidatos, CESPE/UnB, 02/08/2013: http://www.cespe.unb.br/concursos/DPRF_13/arquivos/DEMANDA_DPRF_13.PDF (109.769 inscritos, 1.000 vagas, demanda 109,77)
- Pedido de 533 vagas (269 policial + 264 administrativo) noticiado a partir de ofício da PRF ao MGI; verificado em fontes públicas em 14/07/2026
- Prorrogação da validade do concurso 2021 até 21/12/2026 (DOU)

## Concorrência e abstenção do concurso PRF (2013-2021)

Quantos inscritos tem o concurso da PRF? 304.330 em 2021 (202,9 por vaga), 129.152 em 2018/19 e 109.769 em 2013. Números oficiais de demanda e abstenção.

| ciclo | vagas | inscritos | inscritos_por_vaga | presentes_prova_objetiva | ausentes_prova_objetiva | abstencao_pct |
| --- | --- | --- | --- | --- | --- | --- |
| 2021 | 1500 | 304330 | 202.9 | 205241 | 99089 | 32.6 |
| 2018/19 | 500 | 129152 | 258.3 | – | – | – |
| 2013 | 1000 | 109769 | 109.8 | – | – | – |


**Fontes primárias:**

- Portaria SEDGG/ME nº 25.412 (DOU 24/12/2020)
- Edital nº 1 — PRF 2021, Cebraspe: https://cdn.cebraspe.org.br/concursos/PRF_21/arquivos/ED_1_PRF_2021_ABERTURA.PDF (período de inscrição e cronograma: Anexo I)
- Demanda oficial de candidatos, Cebraspe: https://cdn.cebraspe.org.br/concursos/prf_21/arquivos/PRF_21____DEMANDA_CANDIDATOS_POR_VAGA.PDF (304.330 inscritos, 1.500 vagas)
- Presentes/ausentes na prova objetiva: resultados divulgados pelo Cebraspe/PRF (205.241 presentes, 99.089 ausentes; verificado em fontes públicas em 14/07/2026)
- Portaria MP nº 236 (DOU 27/07/2018)
- Edital de abertura PRF 2018, Cebraspe (cebraspe.org.br/concursos/prf_18)
- Demanda oficial de candidatos, Cebraspe: https://cdn.cebraspe.org.br/concursos/prf_18/arquivos/PRF_18___DEMANDA.PDF (129.152 inscritos, 500 vagas, quebra por UF)
- Edital nº 1 — DPRF 2013, CESPE/UnB (cespe.unb.br/concursos/dprf_13)
- Demanda oficial de candidatos, CESPE/UnB, 02/08/2013: http://www.cespe.unb.br/concursos/DPRF_13/arquivos/DEMANDA_DPRF_13.PDF (109.769 inscritos, 1.000 vagas, demanda 109,77)

## Estrutura da prova da PRF por matéria: blocos oficiais × catálogo de estudo

Legislação de Trânsito é um bloco inteiro sozinha na prova da PRF, com nota mínima própria. Estrutura oficial de 2021 (blocos e notas mínimas) por matéria.

| materia | bloco_edital_2021 | nota_minima_do_bloco | peso_editorial_escuta_policial | aulas_no_catalogo | minutos_de_audio |
| --- | --- | --- | --- | --- | --- |
| Língua Portuguesa | I | 15 | 4 | 6 | 83 |
| Raciocínio Lógico-Matemático | I | 15 | 3 | 6 | 82 |
| Informática | I | 15 | 3 | 3 | 40 |
| Física | I | 15 | 2 | 3 | 37 |
| Ética e Cidadania | I | 15 | 2 | 3 | 35 |
| Geopolítica | I | 15 | 2 | 3 | 37 |
| Língua Estrangeira (Inglês ou Espanhol) | I | 15 | 2 | 2 | 21 |
| Legislação de Trânsito (CTB) | II | 10 | 5 | 12 | 151 |
| Direito Administrativo | III | 10 | 4 | 6 | 72 |
| Direito Constitucional | III | 10 | 4 | 4 | 55 |
| Direito Penal | III | 10 | 4 | 2 | 26 |
| Direito Processual Penal | III | 10 | 3 | 4 | 49 |
| Legislação Especial | III | 10 | 3 | 1 | 11 |
| Direitos Humanos | III | 10 | 3 | 3 | 38 |


**Fontes primárias:**

- Edital nº 1 — PRF, de 2021 (Cebraspe): https://cdn.cebraspe.org.br/concursos/PRF_21/arquivos/ED_1_PRF_2021_ABERTURA.PDF — itens 9 (prova objetiva, critérios 9.12) e 24 (objetos de avaliação, composição dos blocos)
- Peso editorial, aulas e minutos de áudio: catálogo do Escuta Policial (https://escutapolicial.com.br/aulas/), atualizado em 19 de julho de 2026

## 🌡️ Termômetro do Edital PRF - índice diário de aquecimento (0-100)

Índice diário (0-100) de aquecimento do edital da PRF: fase oficial no DOU + sinal de notícias dos últimos 30 dias, com metodologia pública, série histórica e download CSV/JSON. O valor do dia está na própria página.

| data | score | fase_oficial | noticias_30d |
| --- | --- | --- | --- |
| 2026-07-20 | 29 | pre-edital | 6 |
| 2026-07-19 | 29 | pre-edital | 6 |
| 2026-07-18 | 37 | pre-edital | 11 |
| 2026-07-17 | 40 | pre-edital | 13 |
| 2026-07-16 | 40 | pre-edital | 13 |

*Últimos 5 dias - a série completa, um ponto por dia (calendário de Brasília), está no [CSV](datasets/termometro-edital-prf.csv)/[JSON](datasets/termometro-edital-prf.json). Fórmula pública e determinística na [página da metodologia](https://escutapolicial.com.br/dados/termometro-edital-prf/).*

**Fontes primárias:**

- Fase oficial do concurso: monitoramento do Diário Oficial da União pelo robô do Escuta Policial (varredura a cada ~20 minutos, seções 1 e 3)
- Notícias e relevância editorial: Radar PRF do Escuta Policial (escutapolicial.com.br/radar), coleta automatizada 5x/dia de fontes públicas
- Fórmula pública documentada nesta página - índice determinístico, sem IA no cálculo do número

## Salário do Policial Rodoviário Federal: tabela oficial de subsídio (Lei 14.875/2024)

Quanto ganha um Policial Rodoviário Federal? Subsídio inicial de R$ 12.253,84, chegando a R$ 23.000,00 no topo. Tabela da Lei 14.875/2024 em CSV/JSON.

| classe | padrao | subsidio_2024_08 | subsidio_2025_05 | subsidio_2026_05 |
| --- | --- | --- | --- | --- |
| Terceira | I | 11114.6 | 11670.33 | 12253.84 |
| Terceira | II | 11206.08 | 11766.38 | 12440.9 |
| Terceira | III | 11298.47 | 11863.4 | 12630.98 |
| Segunda | I | 13127.22 | 13783.58 | 14764.25 |
| Segunda | II | 13238.83 | 13900.77 | 14993.63 |
| Segunda | III | 13351.55 | 14019.13 | 15226.76 |
| Segunda | IV | 13465.41 | 14138.68 | 15463.72 |
| Segunda | V | 13580.4 | 14259.42 | 15704.54 |
| Segunda | VI | 13696.54 | 14381.37 | 15949.32 |
| Primeira | I | 14712.66 | 15448.3 | 17244.77 |
| Primeira | II | 15095.06 | 15849.82 | 17814.28 |
| Primeira | III | 15488.91 | 16263.36 | 18404.39 |
| Primeira | IV | 15894.59 | 16689.32 | 19015.88 |
| Primeira | V | 16312.45 | 17128.07 | 19649.56 |
| Primeira | VI | 16742.84 | 17579.98 | 20306.21 |
| Especial | I | 17629.42 | 18510.89 | 21524.32 |
| Especial | II | 18099.31 | 19004.28 | 22249.43 |
| Especial | III | 18583.31 | 19512.48 | 23000 |


**Fontes primárias:**

- Lei nº 14.875, de 31 de maio de 2024, Anexo XXVII: https://www2.camara.leg.br/legin/fed/lei/2024/lei-14875-31-maio-2024-795709-anexo-pl.pdf (DOU de 31/05/2024, Seção 1, Edição Extra; texto também em https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2024/lei/L14875.htm)
- Edital nº 1 — PRF, de 18 de janeiro de 2021 (Cebraspe), item 2.3: https://cdn.cebraspe.org.br/concursos/PRF_21/arquivos/ED_1_PRF_2021_ABERTURA.PDF

## TAF da PRF: índices oficiais do teste de aptidão física (edital 2021)

Como é o TAF da PRF? 5 testes eliminatórios (barra fixa, shuttle run, impulsão, abdominal e corrida). Na corrida, o mínimo é 2.301 m (H) e 2.001 m (M).

| teste | sexo | tipo | desempenho | pontos |
| --- | --- | --- | --- | --- |
| Flexão em barra fixa | masculino | reprovado (zero) | 0 a 2 | 0 |
| Flexão em barra fixa | masculino | pontua | 3 | 2 |
| Flexão em barra fixa | masculino | pontua | 4 | 2.5 |
| Flexão em barra fixa | masculino | pontua | 5 | 3 |
| Flexão em barra fixa | masculino | pontua | 6 | 3.5 |
| Flexão em barra fixa | masculino | pontua | 7 | 4 |
| Flexão em barra fixa | masculino | pontua | 8 | 4.5 |
| Flexão em barra fixa | masculino | pontua | 9 ou mais | 5 |
| Flexão em barra fixa | feminino | reprovado (zero) | abaixo de 10 | 0 |
| Flexão em barra fixa | feminino | pontua | 10 a menos de 13 | 2 |
| Flexão em barra fixa | feminino | pontua | 13 a menos de 16 | 2.5 |
| Flexão em barra fixa | feminino | pontua | 16 a menos de 19 | 3 |
| Flexão em barra fixa | feminino | pontua | 19 a menos de 22 | 3.5 |
| Flexão em barra fixa | feminino | pontua | 22 a menos de 25 | 4 |
| Flexão em barra fixa | feminino | pontua | 25 a menos de 28 | 4.5 |
| Flexão em barra fixa | feminino | pontua | 28 ou mais | 5 |
| Shuttle run (ir e vir, 9,14 m) | masculino | reprovado (zero) | 14" ou mais | 0 |
| Shuttle run (ir e vir, 9,14 m) | masculino | pontua | 13"50 a 13"99 | 2 |
| Shuttle run (ir e vir, 9,14 m) | masculino | pontua | 13" a 13"49 | 2.5 |
| Shuttle run (ir e vir, 9,14 m) | masculino | pontua | 12"50 a 12"99 | 3 |
| Shuttle run (ir e vir, 9,14 m) | masculino | pontua | 12" a 12"49 | 3.5 |
| Shuttle run (ir e vir, 9,14 m) | masculino | pontua | 11"50 a 11"99 | 4 |
| Shuttle run (ir e vir, 9,14 m) | masculino | pontua | 11" a 11"49 | 4.5 |
| Shuttle run (ir e vir, 9,14 m) | masculino | pontua | abaixo de 11" | 5 |
| Shuttle run (ir e vir, 9,14 m) | feminino | reprovado (zero) | 16" ou mais | 0 |
| Shuttle run (ir e vir, 9,14 m) | feminino | pontua | 15"50 a 15"99 | 2 |
| Shuttle run (ir e vir, 9,14 m) | feminino | pontua | 15" a 15"49 | 2.5 |
| Shuttle run (ir e vir, 9,14 m) | feminino | pontua | 14"50 a 14"99 | 3 |
| Shuttle run (ir e vir, 9,14 m) | feminino | pontua | 14" a 14"49 | 3.5 |
| Shuttle run (ir e vir, 9,14 m) | feminino | pontua | 13"50 a 13"99 | 4 |
| Shuttle run (ir e vir, 9,14 m) | feminino | pontua | 13" a 13"49 | 4.5 |
| Shuttle run (ir e vir, 9,14 m) | feminino | pontua | abaixo de 13" | 5 |
| Impulsão horizontal | masculino | reprovado (zero) | 0,00 a 2,00 | 0 |
| Impulsão horizontal | masculino | pontua | 2,01 a 2,05 | 2 |
| Impulsão horizontal | masculino | pontua | 2,06 a 2,10 | 2.5 |
| Impulsão horizontal | masculino | pontua | 2,11 a 2,15 | 3 |
| Impulsão horizontal | masculino | pontua | 2,16 a 2,20 | 3.5 |
| Impulsão horizontal | masculino | pontua | 2,21 a 2,25 | 4 |
| Impulsão horizontal | masculino | pontua | 2,26 a 2,30 | 4.5 |
| Impulsão horizontal | masculino | pontua | 2,31 ou mais | 5 |
| Impulsão horizontal | feminino | reprovado (zero) | 0,00 a 1,60 | 0 |
| Impulsão horizontal | feminino | pontua | 1,61 a 1,65 | 2 |
| Impulsão horizontal | feminino | pontua | 1,66 a 1,70 | 2.5 |
| Impulsão horizontal | feminino | pontua | 1,71 a 1,75 | 3 |
| Impulsão horizontal | feminino | pontua | 1,76 a 1,80 | 3.5 |
| Impulsão horizontal | feminino | pontua | 1,81 a 1,85 | 4 |
| Impulsão horizontal | feminino | pontua | 1,86 a 1,90 | 4.5 |
| Impulsão horizontal | feminino | pontua | 1,91 ou mais | 5 |
| Flexão abdominal (1 minuto) | masculino | reprovado (zero) | 0 a 34 | 0 |
| Flexão abdominal (1 minuto) | masculino | pontua | 35 a 38 | 2 |
| Flexão abdominal (1 minuto) | masculino | pontua | 39 a 42 | 2.5 |
| Flexão abdominal (1 minuto) | masculino | pontua | 43 a 46 | 3 |
| Flexão abdominal (1 minuto) | masculino | pontua | 47 a 50 | 3.5 |
| Flexão abdominal (1 minuto) | masculino | pontua | 51 a 54 | 4 |
| Flexão abdominal (1 minuto) | masculino | pontua | 55 a 58 | 4.5 |
| Flexão abdominal (1 minuto) | masculino | pontua | 59 ou mais | 5 |
| Flexão abdominal (1 minuto) | feminino | reprovado (zero) | 0 a 27 | 0 |
| Flexão abdominal (1 minuto) | feminino | pontua | 28 a 30 | 2 |
| Flexão abdominal (1 minuto) | feminino | pontua | 31 a 33 | 2.5 |
| Flexão abdominal (1 minuto) | feminino | pontua | 34 a 36 | 3 |
| Flexão abdominal (1 minuto) | feminino | pontua | 37 a 39 | 3.5 |
| Flexão abdominal (1 minuto) | feminino | pontua | 40 a 42 | 4 |
| Flexão abdominal (1 minuto) | feminino | pontua | 43 a 45 | 4.5 |
| Flexão abdominal (1 minuto) | feminino | pontua | 46 ou mais | 5 |
| Corrida de 12 minutos | masculino | reprovado (zero) | 0 a 2.300 | 0 |
| Corrida de 12 minutos | masculino | pontua | 2.301 a 2.400 | 2 |
| Corrida de 12 minutos | masculino | pontua | 2.401 a 2.500 | 2.5 |
| Corrida de 12 minutos | masculino | pontua | 2.501 a 2.600 | 3 |
| Corrida de 12 minutos | masculino | pontua | 2.601 a 2.700 | 3.5 |
| Corrida de 12 minutos | masculino | pontua | 2.701 a 2.800 | 4 |
| Corrida de 12 minutos | masculino | pontua | 2.801 a 2.900 | 4.5 |
| Corrida de 12 minutos | masculino | pontua | 2.901 ou mais | 5 |
| Corrida de 12 minutos | feminino | reprovado (zero) | 0 a 2.000 | 0 |
| Corrida de 12 minutos | feminino | pontua | 2.001 a 2.100 | 2 |
| Corrida de 12 minutos | feminino | pontua | 2.101 a 2.200 | 2.5 |
| Corrida de 12 minutos | feminino | pontua | 2.201 a 2.300 | 3 |
| Corrida de 12 minutos | feminino | pontua | 2.301 a 2.400 | 3.5 |
| Corrida de 12 minutos | feminino | pontua | 2.401 a 2.500 | 4 |
| Corrida de 12 minutos | feminino | pontua | 2.501 a 2.600 | 4.5 |
| Corrida de 12 minutos | feminino | pontua | 2.601 ou mais | 5 |


**Fontes primárias:**

- Edital nº 1 — PRF, de 18 de janeiro de 2021 (Cebraspe), item 11 e Anexo III: https://cdn.cebraspe.org.br/concursos/PRF_21/arquivos/ED_1_PRF_2021_ABERTURA.PDF

## Requisitos e etapas do concurso da PRF (edital 2021)

Requisitos do concurso PRF: nível superior em qualquer área e CNH B. O edital de 2021 não exigiu idade máxima, altura mínima nem vetou tatuagem. Taxa: R$ 180.

| requisito | exigencia | fonte_oficial |
| --- | --- | --- |
| Escolaridade | Diploma de conclusão de curso de graduação em QUALQUER área de formação, registrado e emitido por instituição reconhecida pelo MEC | Edital 2021, itens 2.1 e 3.3 |
| CNH (habilitação) | Categoria "B" ou superior, válida, sem impedimentos, sem adaptação veicular e sem restrição de locais/horários — exigida também durante todo o Curso de Formação | Edital 2021, itens 3.9 e 13.3-b |
| Idade mínima | 18 anos completos (requisito legal de investidura em cargo público) | Lei nº 8.112/1990, art. 5º, V |
| Idade máxima | Não prevista no edital de 2021 | Edital 2021 (ausência de previsão) |
| Altura mínima | Não prevista no edital de 2021 | Edital 2021 (ausência de previsão) |
| Tatuagem | Permitida. Só reprova tatuagem que viole valores constitucionais: ideologia terrorista/extremista, incitação à violência ou à criminalidade, discriminação ou preconceito | Edital 2021, Anexo V (com base no RE 898.450/SP do STF) |
| Nacionalidade | Brasileira, ou portuguesa amparada pelo Estatuto de Igualdade (CF, art. 12, § 1º) | Edital 2021, item 3.2 |
| Quitações | Estar quite com as obrigações eleitorais e, para homens, com as militares | Edital 2021, itens 3.4 e 3.5 |
| Exame toxicológico | Autorizar a coleta de material para exames toxicológicos a qualquer tempo | Edital 2021, item 3.11 |
| Investigação social | Estende-se durante TODO o concurso, da inscrição à nomeação | Edital 2021, item 1.5 |
| Taxa de inscrição | R$ 180,00 (isenção para inscritos no CadÚnico e doadores de medula óssea) | Edital 2021, item 7.1 |
| Validade do concurso | 2 anos a partir da homologação, prorrogável uma única vez por igual período | Edital 2021, item 23.30 |


**Fontes primárias:**

- Edital nº 1 — PRF, de 18 de janeiro de 2021 (Cebraspe): https://cdn.cebraspe.org.br/concursos/PRF_21/arquivos/ED_1_PRF_2021_ABERTURA.PDF
- Lei nº 8.112/1990, art. 5º (requisitos básicos para investidura em cargo público, inclusive idade mínima de 18 anos)
- STF, Recurso Extraordinário 898.450/SP, de 17/08/2016 (repercussão geral sobre tatuagem em concurso público, citado no Anexo V do edital)

## Notas de corte do concurso PRF 2021: objetiva e final, por lista

Nota de corte da PRF 2021 na ampla concorrência: 73,0 na objetiva, 83,0 no final. Cortes de negros e PCD, com fonte no Cebraspe.

| lista | fase | candidatos | nota_minima | nota_maxima | pontuacao_maxima_da_fase |
| --- | --- | --- | --- | --- | --- |
| ampla-concorrencia | objetiva | 5095 | 73 | 101 | 120 |
| negros | objetiva | 1406 | 69 | 101 | 120 |
| pcd | objetiva | 246 | 50 | 88 | 120 |
| ampla-concorrencia | final (objetiva + discursiva) | 4753 | 83 | 119.93 | 140 |
| negros | final (objetiva + discursiva) | 1257 | 79.06 | 119.93 | 140 |
| pcd | final (objetiva + discursiva) | 180 | 60.77 | 100.4 | 140 |


**Fontes primárias:**

- Edital Concurso PRF nº 11, de 27 de maio de 2021 (Cebraspe) — resultado final na prova objetiva e resultado provisório na prova discursiva: https://cdn.cebraspe.org.br/concursos/prf_21/arquivos/ED_11_PRF_2021_FINAL_OBJETIVA_PROV_DISCURSIVA.PDF
- Edital nº 1 — PRF, de 18 de janeiro de 2021 (Cebraspe) — abertura, itens 4 (vagas), 9.12 (pontuação) e 10.6.1 (limite de correção da discursiva por lista), quadro do item 21 (pontuação máxima do certame): https://cdn.cebraspe.org.br/concursos/PRF_21/arquivos/ED_1_PRF_2021_ABERTURA.PDF
- Edital Concurso PRF nº 12, de 2021 (Cebraspe) — resultado final na prova discursiva e convocação para o exame de aptidão física (TAF): https://cdn.cebraspe.org.br/concursos/prf_21/arquivos/ED_12_PRF_2021_FINAL_DISCURSIVA_CONV_TAF_FIP_MATRCULA.PDF
- Edital Concurso PRF nº 13, de 16 de junho de 2021 (Cebraspe) — retificação, por erro material, da nota final na prova objetiva de uma candidata (inscrição 10031927, nota corrigida para 74,00): https://cdn.cebraspe.org.br/concursos/prf_21/arquivos/ed_13_prf_2021_ret_nota.pdf

## Quem as IAs citam para estudar para a PRF (monitor mensal)

Quais marcas as IAs citam para quem quer estudar para a PRF? Monitor mensal, 5 marcas, metodologia aberta. Última rodada: 19/07/2026.

| data | marca | perguntas_em_que_aparece | total_perguntas | share_of_voice_pct | com_url_citada |
| --- | --- | --- | --- | --- | --- |
| 2026-07-19 | Estratégia Concursos | 13 | 15 | 43.3 | 3 |
| 2026-07-19 | Gran Cursos | 11 | 15 | 36.7 | 2 |
| 2026-07-19 | EmÁudio Concursos | 3 | 15 | 10 | 1 |
| 2026-07-19 | Nova Concursos | 3 | 15 | 10 | 1 |
| 2026-07-19 | Escuta Policial | 0 | 15 | 0 | 0 |


**Fontes primárias:**

- Coleta própria do Escuta Policial via API Anthropic (modelo pinado claude-sonnet-5, busca web habilitada). Painel de perguntas e regras de detecção públicos no dado bruto: https://escutapolicial.com.br/dados/presenca-ia/dados.json

## Como citar

> Escuta Policial - PRF em Números. Dados abertos do concurso da PRF. Disponível em: https://escutapolicial.com.br/dados/ e neste repositório. Compilados de fontes oficiais (DOU, Cebraspe/CESPE). Licença CC BY 4.0.

Mantido por [Escuta Policial](https://escutapolicial.com.br/), plataforma de estudo por áudio para o concurso da PRF. Correções e sugestões: abra uma issue ou pull request.
