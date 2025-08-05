# 🏠 Predição de Valores de Casas na Califórnia

Um projeto de Machine Learning para predição de valores imobiliários utilizando dados do censo da Califórnia.

---

## 📋 Sobre o Projeto

Este projeto implementa um modelo de Machine Learning para predizer valores de casas na Califórnia usando dados demográficos e geográficos. O modelo utiliza técnicas de análise exploratória de dados, pré-processamento e amostragem estratificada para garantir resultados precisos e confiáveis.

### 🎯 Objetivo

Desenvolver um modelo preditivo capaz de estimar o valor mediano das casas em diferentes regiões da Califórnia com base em características como:

- Renda mediana dos moradores
- Idade mediana das casas
- Número de quartos e banheiros
- População local
- Proximidade ao oceano

---

## 🚀 Tecnologias Utilizadas

- **Python 3.x**
- **Pandas** - Manipulação e análise de dados
- **NumPy** - Computação científica
- **Matplotlib** - Visualização de dados
- **Scikit-learn** - Machine Learning
  - `train_test_split` - Divisão dos dados
  - `StratifiedShuffleSplit` - Amostragem estratificada

---

## 📁 Estrutura do Projeto

```
projeto_predição_valor_casas/
│
├── codigo.ipynb           # Notebook principal com análise e modelo
├── senso_california.csv   # Dataset com dados do censo da Califórnia
├── README.md             # Documentação do projeto
└── .git/                 # Controle de versão
```

---

## 📊 Dataset

O dataset `senso_california.csv` contém informações sobre habitações na Califórnia, incluindo:

| Coluna               | Descrição                               |
| -------------------- | --------------------------------------- |
| `longitude`          | Coordenada de longitude                 |
| `latitude`           | Coordenada de latitude                  |
| `housing_median_age` | Idade mediana das casas                 |
| `total_rooms`        | Total de quartos                        |
| `total_bedrooms`     | Total de quartos de dormir              |
| `population`         | População local                         |
| `households`         | Número de domicílios                    |
| `median_income`      | Renda mediana (em dezenas de milhares)  |
| `median_house_value` | Valor mediano das casas (variável alvo) |
| `ocean_proximity`    | Proximidade ao oceano                   |

### 🔍 Características dos Dados

- **Total de registros**: ~20,640 casas
- **Valores ausentes**: 207 registros na coluna `total_bedrooms`
- **Período**: Dados do censo de 1990

---

## 🔧 Instalação e Execução

### Pré-requisitos

- Python 3.7+
- Jupyter Notebook ou VS Code com extensão Python

### 1. Clone o repositório

```bash
git clone https://github.com/giullianoveiga/ML-predicao-de-valores-casa.git
cd ML-predicao-de-valores-casa
```

### 2. Instale as dependências

```bash
pip install pandas matplotlib scikit-learn numpy jupyter
```

### 3. Execute o notebook

```bash
jupyter notebook codigo.ipynb
```

Ou abra o arquivo `codigo.ipynb` no VS Code.

---

## 🧪 Metodologia

### 1. **Análise Exploratória de Dados**

- Carregamento e inspeção inicial dos dados
- Identificação de valores ausentes
- Análise da distribuição das variáveis
- Visualização de histogramas e estatísticas descritivas

### 2. **Pré-processamento**

- Tratamento de valores ausentes
- Criação de categorias de renda para estratificação
- Divisão dos dados em treino e teste (80/20)

### 3. **Amostragem Estratificada**

- Implementação de `StratifiedShuffleSplit`
- Manutenção da proporção das categorias de renda
- Garantia de representatividade nos conjuntos de treino e teste

### 4. **Visualizações**

- Histograma da distribuição de valores das casas
- Análise da distribuição das categorias de renda
- Identificação de padrões e outliers

---

## 📈 Principais Insights

1. **Distribuição de Valores**: A maioria das casas tem valores entre $100k e $500k
2. **Valores Ausentes**: 207 registros (1%) com `total_bedrooms` faltante
3. **Categorias de Renda**: Distribuição não uniforme, com concentração nas faixas médias
4. **Proximidade ao Oceano**: Fator importante na variação de preços

---

## 🎯 Próximos Passos

- [ ] Implementar diferentes algoritmos de ML (Linear Regression, Random Forest, etc.)
- [ ] Realizar feature engineering
- [ ] Implementar validação cruzada
- [ ] Otimizar hiperparâmetros
- [ ] Avaliar métricas de performance (RMSE, MAE, R²)
- [ ] Criar pipeline de preprocessamento
- [ ] Implementar sistema de predição em produção

---

## 👨‍💻 Autor

**Giulliano Veiga**

- 📧 Email: [seu-email@exemplo.com]
- 📱 WhatsApp: (85) 98170-8027
- 💼 LinkedIn: [linkedin.com/in/giullianoveiga]
- 🐙 GitHub: [@giullianoveiga](https://github.com/giullianoveiga)

---

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## 🤝 Contribuições

Contribuições são sempre bem-vindas! Para contribuir:

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

---

## 📚 Referências

- [Scikit-learn Documentation](https://scikit-learn.org/)
- [Pandas Documentation](https://pandas.pydata.org/)
- [California Housing Dataset](https://developers.google.com/machine-learning/crash-course/california-housing-data-description)

---

<div align="center">
  <sub>Feito por <a href="https://github.com/giullianoveiga">Giulliano Veiga</a></sub>
</div>
