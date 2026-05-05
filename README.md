# projeto_exemplo

[![Tests](https://github.com/marciomsm-commits/marciomsm-comits/actions/workflows/tests.yml/badge.svg)](https://github.com/marciomsm-commits/marciomsm-comits/actions/workflows/tests.yml)

Projeto Python de exemplo com estrutura organizada, configuração segura via variáveis de ambiente e testes automatizados.

## Estrutura

```
projeto_exemplo/
├── src/
│   ├── config.py       # Configurações lidas do ambiente
│   ├── main.py         # Ponto de entrada da aplicação
│   └── utils.py        # Funções utilitárias (add, multiply)
├── tests/
│   └── test_utils.py   # Testes com pytest
├── .env.example        # Template de variáveis de ambiente
├── requirements.txt    # Dependências do projeto
└── README.md
```

## Configuração

1. Copie o arquivo de exemplo e preencha com seus valores:
   ```bash
   cp .env.example .env
   ```

2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

## Uso

```bash
python src/main.py
```

## Testes

```bash
pytest tests/ -v
```

## Variáveis de ambiente

| Variável | Descrição | Obrigatória |
|---|---|---|
| `DATABASE_URL` | URL de conexão com o banco de dados | Sim |
| `SECRET_KEY` | Chave secreta da aplicação | Sim |
| `DEBUG` | Ativa modo debug (`true`/`false`) | Não (padrão: `false`) |
