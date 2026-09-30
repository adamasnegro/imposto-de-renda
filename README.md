# 🧾 Imposto de Renda — Organizador de Informações Financeiras

> 📚 **Projeto desenvolvido como desafio prático durante minha jornada de aprendizado na [DIO — Digital Innovation One](https://www.dio.me/).**

Projeto desenvolvido em **Microsoft Excel** com o objetivo de organizar, centralizar e consolidar informações financeiras relacionadas à preparação da declaração de Imposto de Renda.

A proposta consiste em transformar informações que normalmente podem estar distribuídas entre documentos, informes bancários, holerites e anotações em uma **estrutura única, organizada e de fácil consulta**.

Este projeto faz parte da construção do meu **portfólio prático em tecnologia**, colocando em prática conceitos de organização de dados, fórmulas, automação, padronização e documentação.

---

# 🎓 Sobre o Desafio

Este projeto foi desenvolvido a partir de uma proposta prática apresentada durante minha jornada de estudos na **DIO — Digital Innovation One**.

A atividade tem como foco transformar conhecimentos adquiridos durante a formação em uma solução prática, utilizando o **Microsoft Excel** para estruturar informações financeiras.

O desenvolvimento do projeto permitiu trabalhar não apenas com a criação da planilha, mas também com conceitos importantes relacionados à:

* 📊 Organização de dados;
* 🧮 Fórmulas e cálculos;
* 📋 Estruturação de informações;
* 🔄 Automação de tarefas;
* 🗂️ Padronização;
* 🔎 Conferência de informações;
* 🔐 Privacidade e proteção de dados;
* 📝 Documentação de projetos.

> **Objetivo educacional:** desenvolver uma solução funcional a partir de uma necessidade prática, aplicando conhecimentos adquiridos durante a formação.

---

# 🎯 Objetivo do Projeto

A preparação do Imposto de Renda envolve diferentes tipos de informações.

Dados pessoais, informações bancárias, valores financeiros e comprovantes precisam estar organizados para facilitar a conferência e o posterior preenchimento da declaração.

Pensando nesse cenário, o projeto foi estruturado para **centralizar essas informações em uma única planilha**.

### O projeto permite:

* 👤 Organizar os dados do titular;
* 🏦 Registrar informações de diferentes instituições financeiras;
* 💰 Consolidar valores financeiros;
* 📄 Associar informações aos respectivos comprovantes;
* 📅 Registrar entradas financeiras ao longo do período;
* 🧮 Utilizar fórmulas para automatizar cálculos;
* 📋 Padronizar o cadastro de instituições financeiras;
* 🔎 Facilitar a conferência das informações antes da declaração.

---

# 🗂️ Estrutura da Planilha

O arquivo **Imposto de Renda.xlsx** está dividido em quatro abas principais:

```text
📁 Imposto de Renda.xlsx
│
├── 👤 TITULAR
├── 🏦 INFORMES
├── 💳 NOTAS
└── 🏛️ BANCOS
```

Cada aba possui uma responsabilidade específica dentro da organização das informações.

---

# 👤 1. TITULAR

A primeira seção concentra os dados cadastrais do contribuinte.

## Informações disponíveis

| Campo                 | Descrição                                            |
| --------------------- | ---------------------------------------------------- |
| Nome                  | Nome do titular                                      |
| CPF                   | Documento de identificação                           |
| Nascimento            | Data de nascimento                                   |
| Título de Eleitor     | Número do título                                     |
| Cônjuge               | Informação do cônjuge                                |
| Rua                   | Endereço                                             |
| Rua Abreviada         | Forma abreviada do endereço                          |
| CEP                   | Código postal                                        |
| Telefone              | Telefone para contato                                |
| Celular               | Número de celular                                    |
| E-mail                | Endereço eletrônico                                  |
| Alterações            | Indicação de alteração em relação à entrega anterior |
| Dependente Cônjuge    | Informação relacionada ao cônjuge                    |
| Residente do Exterior | Informação de residência                             |

## 💡 Objetivo

A organização dessas informações facilita a localização dos dados cadastrais necessários durante o processo de preparação da declaração.

---

# 🏦 2. INFORMES DE RENDIMENTOS BANCÁRIOS

A segunda seção é dedicada aos dados financeiros provenientes das instituições bancárias.

A estrutura permite cadastrar até três instituições financeiras diretamente na área principal da planilha.

## Informações registradas

Para cada banco são armazenados:

```text
🏦 Instituição financeira
💰 Valor atual
📎 Referência do comprovante
```

### Estrutura

```text
1º Banco
├── Banco
├── Valor Atual
└── Anexo

2º Banco
├── Banco
├── Valor Atual
└── Anexo

3º Banco
├── Banco
├── Valor Atual
└── Anexo
```

---

## 🧮 Consolidação automática

Um dos recursos da planilha é a utilização de fórmula para consolidar os valores registrados nos bancos.

A fórmula utilizada é:

```excel
=SUM(D11,D16,D21)
```

A função realiza a soma dos valores cadastrados nos três bancos.

Dessa forma, quando um dos valores é alterado, o resultado da consolidação é atualizado automaticamente.

### Conceito aplicado

```text
Banco 1 ───────┐
               │
Banco 2 ───────┼──► TOTAL
               │
Banco 3 ───────┘
```

Esse tipo de automação reduz a necessidade de cálculos manuais e ajuda na conferência das informações.

---

# 💳 3. NOTAS — ENTRADAS FINANCEIRAS

A terceira seção foi criada para registrar entradas financeiras ao longo do período.

A estrutura utiliza três informações principais:

| Campo     | Finalidade                           |
| --------- | ------------------------------------ |
| Data      | Identificar quando ocorreu a entrada |
| Categoria | Identificar a origem da receita      |
| Valor     | Registrar o valor recebido           |

### Exemplo

```text
DATA          CATEGORIA       VALOR
30/09/2026    HOLERITE        R$ 3.000,00
```

A estrutura pode ser utilizada para registrar diferentes tipos de entradas financeiras e criar um histórico organizado.

---

# 🏛️ 4. BANCOS

A aba `BANCOS` funciona como uma **base auxiliar** para padronizar as instituições financeiras utilizadas no projeto.

Entre as instituições cadastradas estão:

* Banco do Brasil
* Santander
* Caixa Econômica Federal
* Bradesco
* Itaú Unibanco
* Nubank
* Banco Inter
* Banco Original
* Banco C6
* BTG Pactual
* PagBank
* Mercado Pago
* PicPay
* Sicredi
* Sicoob
* Banrisul
* BRB
* Banco Safra
* Banco BV

A utilização de uma lista separada para os bancos contribui para uma estrutura mais organizada e permite futuras implementações de:

* Listas suspensas;
* Validação de dados;
* Padronização de entradas;
* Expansão da base de instituições.

---

# ⚙️ Recursos Técnicos Utilizados

O projeto utiliza diferentes recursos do Microsoft Excel.

## 📊 Organização estruturada

As informações foram divididas em diferentes abas de acordo com sua finalidade.

```text
TITULAR
   ↓
Dados cadastrais

INFORMES
   ↓
Informações bancárias

NOTAS
   ↓
Entradas financeiras

BANCOS
   ↓
Base auxiliar
```

Essa divisão facilita a navegação e evita concentrar todas as informações em uma única área.

---

## 🧮 Fórmulas

Foi utilizada a função:

```excel
SUM()
```

Para realizar a consolidação automática dos valores financeiros.

Exemplo:

```excel
=SUM(D11,D16,D21)
```

---

## 📋 Base de dados auxiliar

A aba `BANCOS` funciona como uma tabela auxiliar contendo instituições financeiras.

Esse conceito permite separar:

```text
DADOS PRINCIPAIS
        ↓
Informações do contribuinte

DADOS AUXILIARES
        ↓
Lista de instituições
```

Essa organização facilita futuras implementações de validação e seleção de dados.

---

## 📎 Organização de comprovantes

A seção de informes possui campos destinados à identificação dos arquivos utilizados como comprovantes.

Exemplo:

```text
ANEXO
   ↓
BANCOX.PDF
```

A finalidade é facilitar a associação entre o dado registrado na planilha e o documento correspondente.

---

# 🧠 Conceitos Aplicados

Embora o projeto tenha sido desenvolvido em Excel, ele envolve conceitos que também estão presentes em sistemas de informação e desenvolvimento de software.

## 1. Organização de dados

As informações são separadas de acordo com sua finalidade.

## 2. Estruturação

Cada grupo de informações possui uma seção específica.

## 3. Automação

Os cálculos são realizados automaticamente por meio de fórmulas.

## 4. Padronização

A lista de instituições financeiras evita a necessidade de digitar repetidamente os nomes dos bancos.

## 5. Integridade das informações

A organização dos campos facilita a conferência dos dados antes de utilizá-los.

## 6. Rastreabilidade

A referência aos comprovantes ajuda a relacionar uma informação registrada com seu documento de origem.

---

# 🔄 Fluxo de Utilização

O funcionamento da solução pode ser representado da seguinte maneira:

```text
              INÍCIO
                 │
                 ▼
       👤 Cadastrar titular
                 │
                 ▼
       🏦 Registrar instituições
                 │
                 ▼
       💰 Informar valores bancários
                 │
                 ▼
       📎 Associar comprovantes
                 │
                 ▼
       💳 Registrar entradas
                 │
                 ▼
       🧮 Consolidar informações
                 │
                 ▼
       🔎 Conferir os dados
                 │
                 ▼
                FIM
```

---

# 🛠️ Tecnologias e Ferramentas

| Tecnologia/Ferramenta | Utilização                                        |
| --------------------- | ------------------------------------------------- |
| Microsoft Excel       | Desenvolvimento da planilha                       |
| Fórmulas Excel        | Automatização dos cálculos                        |
| Tabelas estruturadas  | Organização das informações                       |
| Listas auxiliares     | Padronização dos bancos                           |
| Documentos PDF        | Referência aos comprovantes                       |
| GitHub                | Versionamento e documentação do projeto           |
| DIO                   | Plataforma de aprendizado e realização do desafio |

---

# 📁 Estrutura do Repositório

A organização sugerida para o projeto no GitHub é:

```text
imposto-de-renda/
│
├── README.md
│
├── Imposto de Renda.xlsx
│
├── documentos/
│   └── comprovantes/
│
└── imagens/
    └── preview-planilha.png
```

> ⚠️ **Importante:** não publique no GitHub dados reais como CPF, endereço, telefone, e-mail, informações bancárias ou documentos pessoais.

Para um repositório público, utilize **dados fictícios ou anonimizados**.

---

# 🔐 Segurança e Privacidade

Este projeto trabalha com informações que podem conter dados pessoais e financeiros.

Por esse motivo, a proteção das informações deve fazer parte do desenvolvimento e da publicação do projeto.

### Nunca publique em um repositório público:

```text
❌ CPF real
❌ Dados bancários reais
❌ Número de conta
❌ Informações de cartão
❌ Endereço residencial completo
❌ Telefone pessoal
❌ Documentos pessoais
❌ Informes de rendimento reais
❌ Comprovantes contendo informações pessoais
```

### Para demonstração:

Utilize:

```text
✅ Dados fictícios
✅ CPF fictício
✅ Bancos de exemplo
✅ Valores simulados
✅ Documentos fictícios
```

Esse cuidado é especialmente importante em projetos publicados no GitHub, pois os arquivos podem ser acessados por terceiros.

---

# 🚀 Possíveis Evoluções

O projeto pode evoluir de uma planilha de organização para uma solução mais completa de controle e análise financeira.

## 📊 Dashboard financeiro

Criar gráficos para visualizar:

* Total por banco;
* Entradas por mês;
* Distribuição das receitas;
* Evolução dos valores;
* Comparativos anuais.

---

## 📅 Controle mensal

Expandir a aba `NOTAS` para registrar todas as entradas do ano:

```text
Janeiro
Fevereiro
Março
Abril
Maio
Junho
Julho
Agosto
Setembro
Outubro
Novembro
Dezembro
```

---

## 🏦 Mais instituições

Permitir o cadastro de uma quantidade maior de bancos e instituições financeiras.

---

## 📎 Controle de documentos

Criar uma estrutura para acompanhar:

```text
Documento
     ↓
Tipo
     ↓
Instituição
     ↓
Data
     ↓
Status
```

---

## 🤖 Automação futura

Uma possível evolução seria integrar diferentes tecnologias:

```text
Excel
   ↓
Python
   ↓
Processamento dos dados
   ↓
Relatórios
   ↓
Dashboard
```

Essa evolução permitiria transformar o projeto em uma aplicação mais completa para organização e análise de informações.

---

# 📚 O que este projeto demonstra

Este projeto demonstra conhecimentos práticos em:

* Organização de informações;
* Estruturação de dados;
* Microsoft Excel;
* Fórmulas;
* Automatização de cálculos;
* Modelagem básica de informações;
* Organização financeira;
* Padronização de dados;
* Documentação técnica;
* Segurança e privacidade de dados.

Além disso, demonstra uma habilidade importante para quem está iniciando na área de tecnologia:

> **Transformar uma necessidade prática em uma solução estruturada.**

---

# 🎓 Aprendizados Durante o Projeto

O desenvolvimento deste desafio permitiu compreender que a criação de uma solução não depende apenas da ferramenta utilizada.

Mesmo utilizando Excel, foi possível trabalhar conceitos importantes de tecnologia.

### Organização é parte da solução

Uma grande quantidade de informações não significa necessariamente que temos uma boa estrutura de dados.

O desafio está em organizar as informações para que sejam:

```text
Fáceis de inserir
       ↓
Fáceis de consultar
       ↓
Fáceis de conferir
       ↓
Fáceis de utilizar
```

### Automação reduz tarefas repetitivas

Uma fórmula simples pode eliminar cálculos manuais e facilitar a atualização das informações.

### Segurança precisa fazer parte do projeto

Ao trabalhar com informações pessoais e financeiras, privacidade e segurança precisam ser consideradas desde a organização até a publicação do projeto.

---

# 🎓 DIO — Digital Innovation One

Este projeto faz parte da minha jornada de aprendizado na **DIO — Digital Innovation One**, plataforma utilizada para desenvolver conhecimentos por meio de cursos, formações, bootcamps e desafios práticos.

A realização de projetos como este permite transformar o conteúdo estudado em **experiência prática e material para construção de portfólio**.

🔗 **DIO:** https://www.dio.me/

---

# ⚠️ Aviso

Este projeto possui finalidade **educacional e de organização de informações**.

A planilha não substitui orientação de contador, profissional tributário ou os sistemas oficiais utilizados para a declaração do Imposto de Renda.

Os dados presentes na versão de demonstração devem ser tratados como **dados fictícios ou anonimizados**.

---

# 👨‍💻 Autor

## Cristiano Bonifácio

Estudante de tecnologia com foco em:

* 🔐 Segurança da Informação
* 🛡️ Cybersecurity
* ☁️ Cloud Computing
* 🐧 Linux
* 🌐 Infraestrutura de TI
* 🐍 Python
* 💻 Desenvolvimento

### 🔗 Conecte-se comigo

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Cristiano%20Bonifácio-blue?style=for-the-badge\&logo=linkedin)](https://www.linkedin.com/in/adamasnegro/)

[![GitHub](https://img.shields.io/badge/GitHub-adamasnegro-black?style=for-the-badge\&logo=github)](https://github.com/adamasnegro)

---

# ⭐ Projeto

Se este projeto foi útil ou interessante para você, considere deixar uma ⭐ no repositório.

Cada projeto representa uma etapa da construção do meu portfólio e da minha evolução na área de tecnologia.

---

# 🚀 Da necessidade à solução

Este projeto começou com uma necessidade prática:

> **Como organizar informações financeiras de maneira estruturada e facilitar sua conferência?**

A resposta foi transformar dados que poderiam estar dispersos em uma estrutura organizada, documentada e preparada para futuras automações.

Esse projeto representa uma etapa da minha jornada de aprendizado na DIO e reforça um princípio que pretendo levar para minha carreira em tecnologia:

> **Identificar problemas, estruturar informações e construir soluções.**

---

<p align="center">
  📚 Projeto desenvolvido como parte da jornada de aprendizado na <strong>DIO — Digital Innovation One</strong>.
</p>
