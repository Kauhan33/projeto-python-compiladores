# Projeto Python — Compiladores (UNA)

Exercícios da disciplina de **Compiladores** (8º período — Centro Universitário UNA),
implementados em Python. Cada exercício une **análise léxica** (tokenização da frase de
entrada) com **análise semântica** (validação do significado + execução da ação),
simulando de forma simplificada duas fases do pipeline de um compilador.

## Projetos

| Projeto | Descrição |
|---|---|
| [Mini-Alexa de Casa Inteligente](UNA/8º%20Periodo/Projeto%20Python/Mini-Alexa%20Casa%20Inteligente) | Assistente que interpreta comandos de voz simulados (ligar/desligar/abrir/fechar/aumentar/diminuir) e valida se a ação faz sentido para o dispositivo. |
| [Analisador de Pedidos da Lanchonete](UNA/8º%20Periodo/Projeto%20Python/Analisador%20Pedidos%20Lanchonete) | Identifica ação, produto e quantidade em pedidos de lanchonete e mantém um carrinho com validação e cálculo de total. |

Cada pasta contém seu próprio `enunciado.md` (transcrito do slide da aula), código-fonte,
testes unitários e um `README.md` com instruções específicas.

## Estrutura comum aos dois projetos

- `lexer.py` — análise léxica: transforma a frase em uma lista de `Token`s classificados
- `semantic.py` — análise semântica: valida o significado dos tokens e executa a ação
- `main.py` — ponto de entrada (modo interativo ou `--demo`)
- `test_*.py` — testes unitários (`python -m unittest ... -v`)
- `README.md` / `enunciado.md` — documentação do exercício

## Como executar

Requer Python 3.10+.

```bash
cd "UNA/8º Periodo/Projeto Python/Mini-Alexa Casa Inteligente"
python main.py            # modo interativo
python main.py --demo     # roda comandos de exemplo
python -m unittest test_mini_alexa.py -v
```

```bash
cd "UNA/8º Periodo/Projeto Python/Analisador Pedidos Lanchonete"
python main.py
python main.py --demo
python -m unittest test_lanchonete.py -v
```

## Repositório

https://github.com/Kauhan33/projeto-python-compiladores
