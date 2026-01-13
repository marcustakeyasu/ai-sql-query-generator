# 🤖 DSA AI SQL Query Generator (Text-to-SQL)

![Python](https://img.shields.io/badge/python-3.12-blue.svg)
![Streamlit](https://img.shields.io/badge/streamlit-app-FF4B4B.svg)
![AI](https://img.shields.io/badge/AI-Gemini_2.0_Flash-orange.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

Este repositório contém um **Assistente de Inteligência Artificial** especializado na geração de consultas SQL a partir de linguagem natural. O projeto foi desenvolvido como um "Projeto Especial" dentro do curso de **SQL Para Análise de Dados e Data Science** da **Data Science Academy (DSA)**.

O objetivo principal é aumentar a produtividade de analistas de dados e cientistas de dados, automatizando a criação de templates complexos e oferecendo explicações didáticas sobre a sintaxe gerada.

---

<img width="1358" height="630" alt="image" src="https://github.com/user-attachments/assets/575e7e18-7a5c-4115-8c71-3676e873243a" />


---

## ⚙️ Funcionalidades

O assistente utiliza o modelo de linguagem de última geração **Gemini 2.0 Flash** para oferecer:

* **Tradução Natural para SQL:** Transforma pedidos como "calcule a média móvel de vendas" em código SQL funcional.
* **Análise de Saída Esperada:** Gera uma visualização tabular fictícia do que a query deve retornar.
* **Explicação Técnica Detalhada:** Detalha cada cláusula (`SELECT`, `JOIN`, `GROUP BY`) e funções avançadas utilizadas.
* **Download Direto:** Permite exportar a consulta gerada para um arquivo `.sql` pronto para uso.

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** [Python 3.12](https://www.python.org/)
* **Interface Web:** [Streamlit](https://streamlit.io/)
* **Motor de IA:** [Google Generative AI (Gemini API)](https://ai.google.dev/)
* **Ambiente:** [Anaconda / Conda](https://www.anaconda.com/)
* **Variáveis de Ambiente:** `python-dotenv` (para proteção de API Keys).

---

## ⚡ Performance e Boas Práticas

Um dos diferenciais deste assistente é a priorização de queries otimizadas. O modelo está instruído a utilizar:

1.  **CTEs (Common Table Expressions):** Para organizar consultas complexas e torná-las mais legíveis.
2.  **Window Functions:** Para cálculos analíticos (médias móveis, rankings) de forma eficiente.
3.  **Foco em Índices:** As queries são estruturadas para tirar proveito de colunas indexadas em bancos de dados de larga escala.

---

## 📂 Estrutura do Repositório

```text
├── dsa_ai_app.py           # Aplicação principal (Streamlit)
├── dsa_resultado_query.sql  # Exemplo de query complexa gerada
├── requirements.txt        # Lista de dependências Python
├── .gitignore              # Proteção para não subir arquivos sensíveis (.env)
└── README.md               # Documentação do projeto

```
## Como Executar o Projeto
### 1. Clonar o Repositório

```bash
git clone [https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git](https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git)
cd NOME_DO_REPOSITORIO
```
### 2. Configurar o Ambiente (Conda)
```bash
# Criação do ambiente virtual
conda create --name dsasqlaigenerator python=3.12 -y

# Ativação do ambiente
conda activate dsasqlaigenerator

# Instalação das dependências
pip install -r requirements.txt
```
### 3. Configurar sua API Key
Crie um arquivo .env na raiz do projeto e adicione sua chave do Google Gemini:
`GOOGLE_API_KEY="AIzaSy..."`

### 4. Iniciar sua Aplicação
```bash
streamlit run dsa_ai_app.py
```

## Exemplos de Prompts
Para testar o potencial da ferramenta, tente:

"Crie uma query SQL para calcular a média de uma coluna com base em duas outras colunas de uma tabela."

"Gere uma consulta que utilize Window Functions para mostrar o ranking de vendas por vendedor em cada região."

## Autor
Marcus Takeyasu <br>
📧 takeyasumarcus@gmail.com <br>
🔗 https://www.linkedin.com/in/takeyasumarcus/
