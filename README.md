# Explorando evolução de código

Neste exercício, iremos explorar a evolução de código em sistemas reais.

Iremos utilizar a ferramenta [GitEvo](https://github.com/andrehora/gitevo).
Essa ferramenta analisa a evolução de código em repositórios Git nas seguintes linguagens: Python, JavaScript, TypeScript e Java.

Você deve submeter via Moodle apenas o link do seu `fork`, conforme descrito abaixo.

# Passo 1: Selecionar repositório a ser analisado

Selecione um repositório relevante na linguagem de sua preferência (Python, JavaScript, TypeScript ou Java).
Você pode encontrar projetos interessantes nos links abaixo:

- Python: https://github.com/topics/python?l=python
- JavaScript: https://github.com/topics/javascript?l=javascript
- TypeScript: https://github.com/topics/typescript?l=typescript
- Java: https://github.com/topics/java?l=java

# Passo 2: Instalar e rodar a ferramenta GitEvo

Instale a ferramenta [GitEvo](https://github.com/andrehora/gitevo) com o comando:

```
pip install gitevo
```

Rode a ferramenta no repositório selecionado através do seguinte comando (dependendo da linguagem do projeto que escolheu):

```shell
# Python
$ gitevo -r python <git_url>

# JavaScript
$ gitevo -r js <git_url>

# TypeScript
$ gitevo -r ts <git_url>

# Java
$ gitevo -r java <git_url>
```

Onde `<git_url>` é URL do repositório a ser analisado.
Por exemplo, para analisar o projeto Flask escrito em Python:

```
$ gitevo -r python https://github.com/pallets/flask
```

# Passo 3: Explorar os gráficos de evolução de código (`index.html`)

Ao rodar a ferramenta [GitEvo](https://github.com/andrehora/gitevo), o arquivo `index.html` é gerado com diversos gráficos de evolução de código.

Abra o arquivo `index.html` e observe com atenção os gráficos gerados.

# Passo 4: Explicar um gráfico de evolução de código

Selecione um dos gráficos de evolução e explique-o com suas palavras.
Por exemplo, você pode:

- Detalhar a evolução ao longo do tempo, 
- Detalhar se as curvas estão de acordo com boas práticas,
- Explicar grandes alterações nas curvas,
- Explorar a documentação do repositório em busca de explicações para grandes alterações
- Etc.

Seja criativo!

# Exercício

Para responder este exercício, primeiramente, você deve fazer um `fork` deste repositório.
No Moodle, você deve submeter apenas a URL do seu `fork`.

Em seguida, adicione o arquivo gerado `index.html` no seu fork.

Por fim, responda as questões abaixo no seu `fork`: 

1. Repositório selecionado: https://github.com/sherlock-project/sherlock

2. Gráfico selecionado: Data structures
  
3. Explicação: O gráfico revela a evolução estratégica no uso de estruturas de dados no projeto sherlock. As listas predominam (23→35 ocorrências), com pico em 2023 (+76%) seguido por otimizações. Tuplas apresentam padrão singular: após queda para 1-2 ocorrências (2021-2024), saltam para 15 em 2025 (+1400%), indicando adoção consciente de imutabilidade. Dicionários mantêm-se estáveis (11±1), refletindo seu papel específico e insubstituível.

Esta trajetória demonstra:
1. Fase inicial de experimentação (2020-2022)
2. Expansão com listas durante crescimento (2023)
3. Maturação com otimizações (2024-2025), especialmente na substituição estratégica de listas por tuplas

A mudança radical em 2025 sugere:
- Adoção de novas políticas de codificação
- Preocupação com performance e segurança de dados
- Possível influência de novas bibliotecas ou membros na equipe

Correlações com outros gráficos:
- Aumento de funções (34→52) criou necessidade por mais estruturas
- Estabilidade em classes (4→10) mostra que o crescimento veio principalmente de código procedural



