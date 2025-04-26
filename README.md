# Chatbot Culinário Brasileiro 🇧🇷🤖

Este é um projeto de chatbot com interface gráfica em Tkinter, que responde a perguntas sobre culinária brasileira. Ele utiliza **NLP com spaCy** e **similaridade semântica** para compreender e responder perguntas relacionadas a pratos típicos, ingredientes, origens e mais.

## 🧠 Tecnologias utilizadas

- [Python 3.10+](https://www.python.org)
- [spaCy](https://spacy.io/) (modelo de linguagem `pt_core_news_md`)
- [NLTK](https://www.nltk.org/)
- [Tkinter](https://wiki.python.org/moin/TkInter)
- [Goose3](https://github.com/goose3/goose3) (para scraping e extração de texto)
- [Scikit-learn](https://scikit-learn.org/stable/) (para TF-IDF e similaridade)
- Arquivos `.txt` com dados de receitas e pratos brasileiros

## ⚙️ Como rodar localmente

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/chatbot-culinario.git
cd chatbot-culinario

python -m venv venv
source venv/bin/activate     # Linux/macOS
venv\Scripts\activate        # Windows


pip install -r requirements.txt
python -m spacy download pt_core_news_md
python main.py

```


 # Exemplos de perguntas
"Quem criou a feijoada?"

"Onde foi originado o acarajé?"

"Quais são os ingredientes da moqueca?"

"Como é preparado o vatapá?"

"O que é o baião de dois?"

# 🔍 Como funciona
O texto do usuário é processado com spaCy (tokenização, lematização, remoção de stopwords).

A pergunta é analisada por palavras-chave e/ou similaridade semântica para entender se ela é sobre:

Origem geográfica

Pessoa que criou

Ingredientes/preparo

# Definição geral

O chatbot então busca no corpus de pratos o texto mais relevante e responde.

# 📌 Observações
O chatbot responde a perguntas gerais sobre culinária brasileira, mas também entende perguntas específicas sobre pratos.

Quanto maior e mais variado o corpus (receitas.txt), mais rico será o vocabulário e as respostas.

