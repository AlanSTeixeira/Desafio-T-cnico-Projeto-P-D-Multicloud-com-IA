# Desafio Técnico – Projeto P&D Multicloud com IA

Este projeto foi desenvolvido como parte do desafio da **Trilha A – Dados & IA (Programa Inova Talentos – ICT Itaú)**, com o objetivo de criar um pipeline simples de ingestão e processamento de dados multicloud a partir de fontes públicas de preços de provedores de nuvem.

## Objetivo

Construir um fluxo de coleta, tratamento e análise de dados de preços de máquinas virtuais (VMs) de diferentes provedores, demonstrando a viabilidade de comparações e previsões para otimização de custos em ambientes multicloud.

## Escopo do Protótipo

Nesta versão, foram integradas duas fontes:

* **Microsoft Azure**
* **Oracle Cloud**

O pipeline realiza:

1. **Coleta de dados** públicos de preços das VMs.
2. **Processamento e limpeza** das informações.
3. **Análise Exploratória de Dados (EDA)** para cada provedor.
4. **Machine Learning** aplicado aos dados da Azure:

   * **Clustering (K-Means)** para identificar padrões de preços por região.
   * **Regressão (Random Forest)** para prever preços com base nas características das VMs.

## Tecnologias Utilizadas

* **Python 3**
* Pandas, NumPy, Matplotlib, Seaborn
* Scikit-learn
* Requests (para coleta via API)
* Jupyter Notebook

## Estrutura do Projeto

```
├── dados/  
│   ├── oracle_vm_prices_tratados.csv  
│   ├── dados_limpos.csv  
├── Desafio_ICT_Itau.ipynb  # Notebook principal  
├── requirements.txt  
├── README.md  
```

## Como Executar

1. **Clone o repositório**

   ```bash
   git clone https://github.com/usuario/repositorio.git
   cd repositorio
   ```

2. **Crie um ambiente virtual (opcional, mas recomendado)**

   ```bash
   python -m venv venv
   source venv/bin/activate   # Linux/Mac
   venv\Scripts\activate      # Windows
   ```

3. **Instale as dependências**

   ```bash
   pip install -r requirements.txt
   ```

4. **Abra o notebook e execute as células na ordem**

   ```bash
   jupyter notebook Desafio_ICT_Itau.ipynb
   ```

## Próximos Passos

* Integrar dados da AWS e GCP.
* Ampliar análise comparativa entre provedores.
* Criar dashboard interativo para visualização dos resultados.

## Licença

Este projeto é de uso acadêmico e experimental, podendo ser adaptado para fins comerciais mediante autorização.
