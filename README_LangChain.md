# Automação de Testes Unitários com LangChain e Azure ChatGPT

## Descrição do Projeto
Este projeto faz parte do desafio da DIO e tem como objetivo utilizar **modelos de linguagem** (Azure ChatGPT) integrados com o **LangChain** para automatizar a criação de testes unitários em Python.  
A proposta é reduzir o tempo gasto na escrita manual de testes e aumentar a cobertura de forma prática.

---

## Objetivos de Aprendizagem
- Aplicar conceitos de IA generativa em cenários práticos.
- Aprender a usar o LangChain para estruturar prompts e fluxos.
- Automatizar a geração de testes unitários.
- Documentar processos técnicos de forma clara e estruturada.
- Compartilhar no GitHub como portfólio técnico.

---

## Configuração do Ambiente

### 1. Pré-requisitos
- Python 3.9+
- Conta no **Azure OpenAI**
- VSCode (ou outro editor de preferência)

### 2. Instalação das dependências
Instale as bibliotecas necessárias:
```bash
pip install langchain openai pytest
```

### 3. Configuração das variáveis de ambiente
Adicione suas credenciais do Azure:
```bash
export OPENAI_API_KEY="sua_chave"
export OPENAI_API_BASE="https://SEU-ENDPOINT.openai.azure.com/"
```

---

## Exemplo Prático

Função simples em Python:
```python
def soma(a, b):
    return a + b
```

Prompt enviado ao modelo (via LangChain):
```
Gere um teste unitário em pytest para a função soma(a, b).
```

Teste gerado automaticamente:
```python
import pytest
from src.main import soma

def test_soma():
    assert soma(2, 3) == 5
    assert soma(-1, 1) == 0
```

Execução dos testes:
```bash
pytest tests/
```

---

## Conclusão
Com esse desafio, aprendi na prática como integrar IA ao processo de desenvolvimento, gerando testes unitários automaticamente.  
Isso pode agilizar bastante o trabalho de desenvolvedores e aumentar a cobertura de testes em projetos reais.

---

## Estrutura do Repositório
```
/src          -> código fonte
/tests        -> testes unitários gerados
/images       -> prints do ambiente (opcional)
README.md     -> documentação do projeto
```
