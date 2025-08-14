# 🧪 Desafio de Programação Python - Avaliação QA

## 📋 Visão Geral

Este desafio foi criado para avaliar as habilidades de programação Python de candidatos à vaga de QA Engineer, com foco em:

- **Manipulação de dados JSON**
- **Trabalho com pandas DataFrames**
- **Análise de dados e identificação de problemas**
- **Criação de frameworks de validação**
- **Geração de relatórios de qualidade**

## 🎯 Objetivos do Desafio

O candidato deve demonstrar capacidade de:

1. **Analisar dados** de vendas em formato JSON
2. **Identificar problemas** e inconsistências nos dados
3. **Criar validações** automatizadas
4. **Gerar insights** e relatórios úteis
5. **Implementar soluções** reutilizáveis

## 📁 Estrutura do Projeto

```
avaliacaoQA/
├── desafio_qa_python.ipynb    # Jupyter Notebook com o desafio
├── dados_vendas.json          # Dados de exemplo 
└── README.md                  # Este arquivo
```

## 🚀 Como Usar

### Pré-requisitos

```bash
# Instalar dependências
pip install pandas numpy jupyter matplotlib seaborn

# Ou usando conda
conda install pandas numpy jupyter matplotlib seaborn
```

### Opções de Execuão

Você pode utilizar o ambiente de sua preferência para resolver o desafio:
Jupyter Notebook (via navegador): basta rodar jupyter notebook no terminal e abrir o arquivo desafio_qa_python.ipynb

VS Code com a extensão Jupyter: abra o notebook diretamente no VS Code e execute as células normalmente
Certifique-se de que o ambiente tenha Python 3 instalado e as bibliotecas necessárias (como pandas, numpy, matplotlib, etc.).

### Executando o Desafio com Juypter

1. **Clone ou baixe** os arquivos do projeto
2. **Abra o Jupyter Notebook:**
   ```bash
   jupyter notebook desafio_qa_python.ipynb
   ```
3. **Use o notebook como base para sua solução** — as instruções estão neste `README.md`

## 🧩 Sobre os Dados

Você receberá um arquivo `dados_vendas.json` com um conjunto de registros de vendas. Espera-se que você faça uma análise detalhada, identifique eventuais problemas ou inconsistências e proponha melhorias baseadas em validações automatizadas.

Não indicaremos previamente os problemas — parte da sua análise envolve investigá-los e classificá-los criticamente.


## 📊 Critérios de Avaliação

### **Nível Básico (0-60 pontos)**
- ✅ Carrega dados JSON corretamente
- ✅ Converte para DataFrame
- ✅ Identifica problemas óbvios
- ✅ Código funcional

### **Nível Intermediário (60-80 pontos)**
- ✅ Análise exploratória completa
- ✅ Validações funcionais
- ✅ Relatórios básicos
- ✅ Código bem estruturado

### **Nível Avançado (80-100 pontos)**
- ✅ Framework de validação reutilizável
- ✅ Análises avançadas e insights
- ✅ Tratamento robusto de erros
- ✅ Documentação clara
- ✅ Recomendações práticas

## 🏆 Habilidades Avaliadas

### **Técnicas**
- Manipulação de JSON e DataFrames
- Análise de dados com pandas
- Programação orientada a objetos
- Tratamento de exceções

### **Soft Skills**
- Análise crítica de problemas
- Comunicação técnica
- Pensamento sistêmico
- Documentação

### **Visão de Negócio**
- Impacto dos problemas identificados
- Recomendações práticas
- Melhorias no processo

## 📝 Dicas para o Candidato

1. **Leia atentamente** todas as instruções
2. **Teste seu código** antes de finalizar
3. **Documente suas decisões** e raciocínio
4. **Pense no impacto** dos problemas encontrados
5. **Mantenha o código limpo** e bem estruturado
6. **Não se esqueça** da parte de documentação

## 🔍 Exemplo de Solução Esperada

O candidato deve ser capaz de:

```python
# Exemplo de validação esperada
def detectar_precos_negativos(df):
    """Detecta registros com preços negativos ou zero"""
    problemas = df[df['preco'] <= 0]
    return problemas

# Exemplo de análise esperada
def analisar_vendas_por_categoria(df):
    """Analisa vendas agrupadas por categoria"""
    return df.groupby('categoria').agg({
        'quantidade': 'sum',
        'preco': lambda x: (x * df.loc[x.index, 'quantidade']).sum()
    }).rename(columns={'preco': 'receita_total'})
```

## 📞 Suporte

Se houver dúvidas sobre o desafio, entre em contato com a equipe de recrutamento.

---

## 💡 Observações Importantes

- Você pode usar recursos que normalmente usaria no dia a dia, como documentação oficial, bibliotecas externas e referências online.
- **Porém, é essencial que você entenda o que está fazendo** — no dia da apresentação poderá ser solicitado que você explique partes do seu código ou implemente melhorias ao vivo.



**Boa sorte! 🚀** 