# Análise de Clusterização de Clientes por Comportamento de Compra

## 📌 Visão Geral do Projeto
Este projeto tem como objetivo segmentar clientes em grupos homogêneos (clusters) com base em seu comportamento de compra, utilizando técnicas de machine learning não supervisionado. A segmentação permitirá a criação de campanhas de marketing personalizadas e estratégias de vendas mais eficientes.

## 🛠️ Tecnologias Utilizadas
- **Linguagens**: Python, SQL
- **Ferramentas**: Google Colab, Jupyter Notebook
- **Bibliotecas**: Pandas, NumPy, SciKit-Learn, Matplotlib, Seaborn
- **Métodos**: Clusterização (K-Means, DBSCAN, Hierarchical Clustering), Análise Exploratória de Dados (EDA), Pré-processamento de Dados

## 📊 Conjunto de Dados
O dataset inicial contém transações de vendas com as seguintes colunas:

| Coluna       | Descrição                          | Tipo      |
|--------------|------------------------------------|-----------|
| InvoiceNo    | Identificação única da transação   | Inteiro   |
| StockCode    | Código do produto em estoque       | String    |
| Description  | Descrição detalhada do produto     | String    |
| Quantity     | Quantidade de itens por transação  | Inteiro   |
| InvoiceDate  | Data e hora da transação           | DateTime  |
| UnitPrice    | Preço unitário do produto          | Float     |
| CustomerID   | Identificação única do cliente     | Inteiro   |
| Country      | País de origem da transação        | String    |

## 🚀 Etapas do Projeto

### 1️⃣ Análise Exploratória de Dados (EDA)
- Identificação de valores ausentes e outliers
- Análise de distribuição das variáveis quantitativas
- Visualização de relações entre variáveis
- Análise de frequência de compras por país/cliente

### 2️⃣ Pré-processamento de Dados
- Tratamento de missing values (CustomerID, Description)
- Normalização/padronização das features
- Engenharia de features:
  - RFM (Recência, Frequência, Valor Monetário)
  - Média de itens por compra
  - Preferência por categoria de produto
- Codificação de variáveis categóricas

### 3️⃣ Seleção do Algoritmo de Clusterização
- Avaliação de diferentes abordagens:
  - K-Means (com método do cotovelo para determinar K ideal)
  - DBSCAN (para detecção de outliers)
  - Agglomerative Clustering
- Validação da qualidade dos clusters (Silhouette Score, Davies-Bouldin Index)

### 4️⃣ Análise dos Clusters Obtidos
- Caracterização de cada cluster:
  - Perfil de compra médio
  - Valor monetário agregado
  - Frequência de compras
  - Produtos preferidos
- Visualização multidimensional (PCA/t-SNE)

### 5️⃣ Interpretação dos Resultados
- Nomeação dos clusters baseada em características dominantes
  - Ex: "Clientes Premium", "Compradores Ocasais", "Caçadores de Ofertas"
- Recomendações de estratégias de marketing para cada segmento
- Análise de potencial de upsell/cross-sell por cluster

## 📈 Resultados Esperados
![Exemplo de Visualização de Clusters](https://github.com/user-attachments/assets/3ecad0b0-6283-4950-ba81-87f1b3b56f02)

- Segmentação clara dos clientes em grupos com comportamentos distintos
- Insights acionáveis para a equipe de marketing
- Aumento potencial na conversão de campanhas direcionadas

## 🏁 Como Executar
1. Clone o repositório
   ```bash
   git clone https://github.com/seu-usuario/projeto-clusterizacao-clientes.git
   ```
2. Execute os notebooks na ordem numérica

## 🤝 Contribuição
Contribuições são bem-vindas! Siga o fluxo:
1. Faça um fork do projeto
2. Crie sua branch (`git checkout -b feature/nova-feature`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/nova-feature`)
5. Abra um Pull Request
