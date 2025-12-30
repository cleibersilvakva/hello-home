# Hello Home

Bem-vindo ao **Hello Home**! Este é um projeto full-stack moderno e leve, desenvolvido para demonstrar a integração entre um backend poderoso em Python e um frontend responsivo.

## 🚀 Sobre o Projeto

O **Hello Home** é uma aplicação web que combina:
*   **Backend:** Uma API rápida construída com **FastAPI**.
*   **Frontend:** Uma interface limpa e moderna (HTML5/CSS3/JS) servida estaticamente pelo próprio backend.
*   **Gerenciamento:** Utiliza o **uv**, a ferramenta mais rápida atualmente para gerenciamento de pacotes e projetos Python.

### Funcionalidades Atuais

1.  **API REST:**
    *   Endpoint `/api/hello`: Retorna uma mensagem JSON de boas-vindas.
2.  **Frontend Dinâmico:**
    *   Consome a API para exibir o status do servidor em tempo real.
    *   Exibe imagens aleatórias de alta qualidade (via Unsplash) a cada recarregamento.
    *   Design moderno com sombras suaves, tipografia "Inter" e layout responsivo (Card UI).
3.  **Automação:**
    *   O servidor verifica e cria automaticamente a estrutura de pastas (`static/`) e o arquivo `index.html` caso eles não existam na inicialização.

## 🛠 Tecnologias Utilizadas

*   Python 3.12+
*   FastAPI - Framework web moderno e de alta performance.
*   Uvicorn - Servidor ASGI para produção.
*   uv - Gerenciador de pacotes e projetos ultra-rápido.

## 📂 Estrutura do Projeto

```text
hello-home/
├── main.py           # Ponto de entrada da aplicação (Servidor e Lógica)
├── pyproject.toml    # Configuração do projeto e dependências (uv)
├── uv.lock           # Arquivo de bloqueio de versões (garante reprodutibilidade)
└── static/           # Arquivos estáticos (Frontend)
    └── index.html    # Página principal (gerada automaticamente ou editável)
```

## ⚡ Como Rodar o Projeto

### Pré-requisitos

Certifique-se de ter o **uv** instalado. Se não tiver, instale-o (Linux/macOS):
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

### Passo a Passo

1.  **Clone o repositório (se ainda não tiver):**
    ```bash
    git clone https://github.com/SEU_USUARIO/hello-home.git
    cd hello-home
    ```

2.  **Instale as dependências e rode o servidor:**
    Com o `uv`, você não precisa criar ambientes virtuais manualmente. Basta rodar:
    ```bash
    uv run main.py
    ```

3.  **Acesse no navegador:**
    Abra http://localhost:8000 para ver o frontend.
    Acesse http://localhost:8000/docs para ver a documentação automática da API (Swagger UI).