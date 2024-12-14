# Sistema de Análise e Previsão de Séries Temporais

Este repositório contém um sistema desenvolvido em **Python** e **Streamlit** para análise e previsão de séries temporais utilizando o modelo **SARIMAX**.

## Estrutura do Projeto

```
project-series-temporais/
|├── .streamlit/
|   └── config.toml            # Configurações do Streamlit
|├── milk.py                   # Código principal do aplicativo
|├── monthly-milk-production-pounds-p.csv  # Exemplo de base de dados
|├── poetry.lock               # Arquivo de dependências gerenciado pelo Poetry
|├── pyproject.toml             # Configuração do projeto Poetry
└── requirements.txt           # Lista de dependências do projeto
```

## Funcionalidades

O sistema permite:

1. **Upload de Arquivos**: Permite ao usuário fazer upload de arquivos `.csv` contendo a série temporal.
2. **Definição de Período Inicial**: Usuário define a data inicial da série.
3. **Previsão com SARIMAX**: Gera previsões para um número definido de meses à frente (1 a 48 meses).
4. **Visualização**:
   - Decomposição da Série Temporal (tendência, sazonalidade e residuais).
   - Gráfico com previsões.
   - Tabela com os valores previstos.

## Como Executar o Projeto

### 1. Clonar o Repositório

```bash
git clone <URL_DO_REPOSITORIO>
cd project-series-temporais
```

### 2. Instalar Dependências

#### Usando `requirements.txt`:

```bash
pip install -r requirements.txt
```

#### Usando `Poetry`:

```bash
poetry install
```

### 3. Executar o Sistema

```bash
streamlit run milk.py
```

O aplicativo estará disponível no navegador em `http://localhost:8501`.

## Exemplo de Uso

Carregue um arquivo `.csv` com uma única coluna representando a série temporal (exemplo: produção mensal de leite). O sistema processará a série e:

- Exibirá a decomposição da série temporal.
- Gerará previsões utilizando o modelo SARIMAX.
- Disponibilizará gráficos e os valores previstos em formato tabular.

## Exemplo de Arquivo `.csv`

```
1234
1320
1410
1500
...
```

## Contato

Caso tenha dúvidas ou sugestões, sinta-se à vontade para  entrar em contato.

---

**Licença**: Este projeto está sob a licença MIT.

