# 📊 Dados abertos - Concurso PRF 2026 (Polícia Rodoviária Federal)

> Fatos do concurso da PRF compilados de **fontes primárias** (Diário Oficial da União, editais e PDFs oficiais do Cebraspe/CESPE) e atualizados automaticamente: um robô do [Escuta Policial](https://escutapolicial.com.br/dados/) lê o DOU a cada ~20 minutos e este repositório é espelhado a cada varredura do Radar (5x por dia).

**🌡️ Termômetro do Edital PRF em 16/07/2026: `38/100` - em aquecimento** · fase oficial: pre-edital · [metodologia](https://escutapolicial.com.br/dados/termometro-edital-prf/)

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

## Linha do tempo real dos concursos da PRF (2013-2026)

Quanto tempo entre a autorização, o edital e a prova da PRF? Dataset com as datas oficiais dos concursos de 2013, 2018/19 e 2021: o edital saiu 26 dias (2021) e 124 dias (2018/19) após a autorização.

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

Quantos inscritos tem o concurso da PRF? 304.330 em 2021 (202,9 por vaga), 129.152 em 2018/19 e 109.769 em 2013 - dataset com os números oficiais de demanda e abstenção.

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

Legislação de Trânsito é um bloco inteiro sozinha na prova da PRF, com nota mínima própria. Dataset com a estrutura oficial da prova de 2021 (blocos e mínimos) cruzada com o catálogo de áudio-aulas por matéria.

| materia | bloco_edital_2021 | nota_minima_do_bloco | peso_editorial_escuta_policial | aulas_no_catalogo | minutos_de_audio |
| --- | --- | --- | --- | --- | --- |
| Língua Portuguesa | I | 15 | 4 | 6 | 83 |
| Raciocínio Lógico-Matemático | I | 15 | 3 | 6 | 82 |
| Informática | I | 15 | 3 | 3 | 40 |
| Física | I | 15 | 2 | 3 | 37 |
| Ética e Cidadania | I | 15 | 2 | 3 | 35 |
| Geopolítica | I | 15 | 2 | 3 | 37 |
| Língua Estrangeira | I | 15 | 2 | 2 | 21 |
| Legislação de Trânsito (CTB) | II | 10 | 5 | 12 | 151 |
| Direito Administrativo | III | 10 | 4 | 6 | 72 |
| Direito Constitucional | III | 10 | 4 | 4 | 55 |
| Direito Penal | III | 10 | 4 | 2 | 26 |
| Direito Processual Penal | III | 10 | 3 | 4 | 49 |
| Legislação Especial | III | 10 | 3 | 1 | 11 |
| Direitos Humanos | III | 10 | 3 | 3 | 41 |


**Fontes primárias:**

- Edital nº 1 — PRF, de 2021 (Cebraspe): https://cdn.cebraspe.org.br/concursos/PRF_21/arquivos/ED_1_PRF_2021_ABERTURA.PDF — itens 9 (prova objetiva, critérios 9.12) e 24 (objetos de avaliação, composição dos blocos)
- Peso editorial, aulas e minutos de áudio: catálogo do Escuta Policial (https://escutapolicial.com.br/aulas/), atualizado em 16 de julho de 2026

## 🌡️ Termômetro do Edital PRF - índice diário de aquecimento (0-100)

Índice diário (0-100) de aquecimento do edital da PRF: fase oficial no DOU + sinal de notícias dos últimos 30 dias, com metodologia pública, série histórica e download CSV/JSON. O valor do dia está na própria página.

| data | score | fase_oficial | noticias_30d |
| --- | --- | --- | --- |
| 2026-07-16 | 38 | pre-edital | 12 |

*Últimos 1 dias - a série completa, um ponto por dia (calendário de Brasília), está no [CSV](datasets/termometro-edital-prf.csv)/[JSON](datasets/termometro-edital-prf.json). Fórmula pública e determinística na [página da metodologia](https://escutapolicial.com.br/dados/termometro-edital-prf/).*

**Fontes primárias:**

- Fase oficial do concurso: monitoramento do Diário Oficial da União pelo robô do Escuta Policial (varredura a cada ~20 minutos, seções 1 e 3)
- Notícias e relevância editorial: Radar PRF do Escuta Policial (escutapolicial.com.br/radar), coleta automatizada 5x/dia de fontes públicas
- Fórmula pública documentada nesta página - índice determinístico, sem IA no cálculo do número

## Como citar

> Escuta Policial - PRF em Números. Dados abertos do concurso da PRF. Disponível em: https://escutapolicial.com.br/dados/ e neste repositório. Compilados de fontes oficiais (DOU, Cebraspe/CESPE). Licença CC BY 4.0.

Mantido por [Escuta Policial](https://escutapolicial.com.br/), plataforma de estudo por áudio para o concurso da PRF. Correções e sugestões: abra uma issue ou pull request.
