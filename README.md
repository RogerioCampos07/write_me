# LangGraph Agent Template 🚀

Este é um template profissional e estruturado para o desenvolvimento, estudo e deploy de agentes autônomos utilizando **LangGraph**, **Python 3.14+** e **Poetry**. O projeto foi desenhado seguindo as melhores práticas de mercado e DevOps, contando com arquitetura multi-stage em Docker para garantir builds leves e eficientes.

## 📌 Estrutura do Projeto

A estrutura de arquivos segue o padrão moderno para aplicações Python modulares:

```text
TEMPLATE_AGENT/
├── template_agent/       # Código fonte principal do agente
│   ├── __init__.py       # Inicialização do módulo
│   └── settings.py       # Gerenciamento de configurações e variáveis de ambiente
├── tests/                # Testes automatizados (Pytest)
│   └── __init__.py
├── .dockerignore         # Arquivos ignorados no contexto do Docker
├── .env-example          # Modelo de variáveis de ambiente obrigatórias
├── .gitignore            # Arquivos ignorados pelo Git
├── Dockerfile            # Build otimizado em múltiplos estágios (Multi-stage Build)
├── poetry.lock           # Travamento de versões exatas das dependências
├── pyproject.toml        # Configuração do projeto, metadados e dependências (Poetry)
└── README.md             # Documentação oficial do projeto
```

---

## 🛠️ Pré-requisitos

Antes de começar, certifique-se de ter instalado em sua máquina local:

* Python 3.14+

* Poetry

* Docker

## 🚀 Instalação e Configuração Local

1 Clone o repositório ou navegue até o diretório do projeto:

```bash
cd TEMPLATE_AGENT
```

2 Configure as Variáveis de Ambiente:
Copie o arquivo de exemplo e preencha com as suas chaves de API (ex: OpenAI, Anthropic, Google Gemini, LangChain API, etc.):

```bash
cp .env-example .env
```

3 Instale as dependências com o Poetry:
O Poetry gerenciará o ambiente virtual isolado de desenvolvimento automaticamente.

```bash
poetry install
```

4 Ative o ambiente virtual:

```bash
source .venv/bin/activate
```

---

## 🧼 Ferramentas de Qualidade de Código

O template já está pré-configurado para utilizar o Ruff para linting e formatação extremamente rápidos.

```bash
task format
```

obs: Veja outros shortcuts de comandos e outras ferramentas no arquivo **pyproject.toml**

## 🧠 Fluxo de Desenvolvimento com LangGraph

1 Defina suas variáveis e tokens de provedores de LLM no arquivo .env.

2 Centralize as configurações globais do sistema de agentes e carregamento do Pydantic no template_agent/settings.py.

3 Crie os estados (State), nós (Nodes) e as bordas (Edges) do seu grafo dentro do pacote template_agent/.

4 Monitore e depure a execução de seus grafos integrando o projeto ao LangSmith ou LangGraph Studio.
