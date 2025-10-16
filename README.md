# Checkpoint 3 - Analise de Dados do ONS

---
## Ddownload do arquivo .ipynb com os códigos:
[Baixar CAPACIDADE_GERACAO.csv](https://github.com/SEU_USUARIO/SEU_REPOSITORIO/raw/main/data/CAPACIDADE_GERACAO.csv)

---
### Integrantes
- Arthur Marangoni Furlan | RM: 564665
- Vinicius Macedo Carvalho | RM: 563791
- Gustavo Sartori Shibata Grigoletto | RM: 565726

## Objetivo
Este notebook tem como finalidade analisar dados públicos do **Operador Nacional do Sistema Elétrico (ONS)**, aplicando técnicas de **análise de dados** e **aprendizado de máquina** em Python.

O arquivo utilizado, `CAPACIDADE_GERACAO.csv`, contém informações sobre:
- Tipo de geração (hidráulica, solar, eólica, térmica etc.);
- Capacidade instalada (em MW);
- Data de início de operação;
- Estado de localização da usina.

---

## Etapas da Análise
1. **Importação e tratamento dos dados**  
   - Leitura e limpeza do arquivo `CAPACIDADE_GERACAO.csv`;  
   - Conversão de colunas para formatos adequados (datas e valores numéricos);  
   - Remoção de dados ausentes e inconsistentes.

2. **Exploração e visualização**  
   - Geração de gráficos e tabelas com a evolução da capacidade instalada;  
   - Comparação entre diferentes fontes de energia por estado e ao longo do tempo.

3. **Modelagem e Machine Learning**  
   - Regressão linear para prever o crescimento da energia solar;  
   - Random Forest para classificação de tipos de usinas;  
   - K-Means para agrupamento de usinas por perfil.

4. **Interpretação dos resultados**  
   - Análise das tendências da matriz elétrica brasileira;  
   - Discussão dos padrões e previsões obtidos com os modelos.

---

## Bibliotecas utilizadas
- `pandas` — manipulação e tratamento de dados  
- `matplotlib` e `seaborn` — visualização gráfica  
- `numpy` — cálculos numéricos  
- `scikit-learn` — aprendizado de máquina (modelagem, classificação e clusterização)

---

## Execução
Certifique-se de que o arquivo **CAPACIDADE_GERACAO.csv** está no mesmo diretório do notebook ou dentro da pasta `data/`.  
No **Google Colab**, utilize o seguinte comando para importar o arquivo manualmente:

```python
from google.colab import files
uploaded = files.upload()
filename = list(uploaded.keys())[0]
```


---

## 🧩 **Conclusões (para o final do notebook)**

```markdown```
# 🧩 Conclusões da Análise

---

## 📈 Síntese dos Resultados

1. **Diversificação da Matriz Energética**
   - O Brasil possui uma matriz energética altamente diversificada.
   - A geração **hidrelétrica** ainda domina, mas as fontes **solar** e **eólica** apresentaram crescimento expressivo na última década.

2. **Evolução das Fontes Renováveis**
   - A energia **solar** foi a que mais cresceu, refletindo o avanço da tecnologia fotovoltaica e os incentivos à energia distribuída.
   - A **energia eólica** consolidou-se no **Nordeste**, com destaque para os estados do **Rio Grande do Norte** e **Bahia**.

3. **Correlação Geográfica**
   - A geração **hidrelétrica** se concentra nas regiões **Norte e Centro-Oeste**.  
   - A geração **solar** se expande principalmente no **Sudeste**, onde há maior densidade populacional e consumo.

4. **Modelos Preditivos**
   - O modelo de **Regressão Linear** mostrou um **crescimento linear contínuo** da capacidade solar para os próximos cinco anos.  
   - Isso sugere estabilidade e consolidação da expansão do setor renovável no país.

5. **Classificação e Clusterização**
   - O modelo **Random Forest** obteve boa acurácia, destacando que **potência instalada** e **estado** são os fatores mais determinantes na classificação das usinas.  
   - O **K-Means** identificou grupos bem definidos:
     - **Cluster 0:** pequenas eólicas e solares recentes;  
     - **Cluster 1:** médias hidráulicas e térmicas;  
     - **Cluster 2:** grandes hidrelétricas mais antigas.

---

## 🌿 Conclusão Geral
O estudo evidencia que a **transição energética brasileira** está em pleno curso, com destaque para o avanço das fontes **solar e eólica**.  
As análises e modelos aplicados demonstram o potencial do **machine learning** como ferramenta para:
- **Prever tendências de expansão** da matriz elétrica;  
- **Identificar padrões regionais** de geração;  
- **Apoiar decisões estratégicas** no setor de energia renovável.

Esses resultados reforçam o papel central das **energias limpas e sustentáveis** no futuro do Brasil, alinhando crescimento econômico com responsabilidade ambiental.

---

## 📚 Referências
- Operador Nacional do Sistema Elétrico (ONS) — Portal de Dados Abertos  
- Agência Nacional de Energia Elétrica (ANEEL)  
- Python Software Foundation — Documentação Oficial  
- Scikit-learn Documentation — Machine Learning API  
