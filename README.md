# 🧾 Imposto de Renda — Organizador de Informações Financeiras

> 📊 Projeto desenvolvido em Excel para organizar, centralizar e consolidar informações necessárias à preparação da declaração de Imposto de Renda.

Este projeto foi desenvolvido com o objetivo de transformar informações financeiras que normalmente ficam espalhadas entre documentos, informes bancários, holerites e anotações em uma **estrutura única, organizada e de fácil consulta**.

A proposta é utilizar o Excel como uma ferramenta de apoio à organização dos dados, permitindo registrar informações do titular, instituições financeiras, valores bancários e entradas financeiras ao longo do período.

---

## 🎯 Objetivo do Projeto

A preparação do Imposto de Renda exige atenção a diferentes tipos de informações.

Dados pessoais, informações bancárias, valores financeiros e comprovantes precisam estar organizados para facilitar a conferência e o preenchimento da declaração.

Pensando nesse cenário, este projeto foi estruturado para centralizar essas informações em uma única planilha.

### O projeto permite:

* 👤 Organizar os dados do titular;
* 🏦 Registrar informações de diferentes instituições bancárias;
* 💰 Consolidar valores financeiros;
* 📄 Associar informações aos respectivos comprovantes;
* 📅 Registrar entradas financeiras ao longo do período;
* 🧮 Utilizar fórmulas para automatizar cálculos;
* 📋 Padronizar o cadastro de instituições financeiras;
* 🔎 Facilitar a conferência das informações antes da declaração.

---

# 🗂️ Estrutura da Planilha

O arquivo está dividido em quatro abas principais:

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

### Informações disponíveis

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
| Dependente Cônjuge    | Indicação relacionada ao cônjuge                     |
| Residente do Exterior | Informação de residência                             |

### 💡 Objetivo

A organização dessas informações facilita a localização dos dados cadastrais necessários durante o processo de preenchimento da declaração.

---

# 🏦 2. INFORMES DE RENDIMENTOS BANCÁRIOS

A segunda seção é dedicada aos dados financeiros provenientes das instituições bancárias.

A estrutura permite cadastrar até três instituições financeiras diretamente na área principal.

### Informações registradas

Para cada banco são armazenados:

```text
🏦 Instituição financeira
💰 Valor atual
📎 Referência do comprovante
```

Exemplo da estrutura:

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

Um dos recursos interessantes da planilha é a utilização de fórmula para consolidar os valores registrados nos bancos.

A fórmula utilizada é:

```excel
=SUM(D11,D16,D21)
```

Ela soma os valores cadastrados nos três bancos.

Isso permite que o total seja atualizado automaticamente quando os valores individuais forem alterados.

### Conceito aplicado

```text
Banco 1 ───────┐
               │
Banco 2 ───────┼──► TOTAL
               │
Banco 3 ───────┘
```

Esse tipo de automação reduz a necessidade de realizar cálculos manualmente.

---

# 💳 3. NOTAS BANCÁRIAS E ENTRADAS

A terceira seção foi criada para registrar as entradas financeiras ao longo do período.

A estrutura utiliza três informações principais:

| Campo     | Finalidade                           |
| --------- | ------------------------------------ |
| Data      | Identificar quando ocorreu a entrada |
| Categoria | Identificar a origem da receita      |
| Valor     | Registrar o valor recebido           |

Exemplo:

```text
DATA          CATEGORIA       VALOR
30/09/2026    HOLERITE        R$ 3.000,00
```

A estrutura pode ser utilizada para registrar diferentes tipos de entradas financeiras, permitindo criar um histórico organizado.

---

# 🏛️ 4. BANCOS

A aba `BANCOS` funciona como uma base de apoio para padronizar as instituições financeiras utilizadas no projeto.

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

A utilização de uma lista separada para os bancos permite manter uma estrutura mais organizada e facilita futuras implementações de listas suspensas e validações de dados.

---

# ⚙️ Recursos Técnicos Utilizados

O projeto utiliza conceitos importantes do Microsoft Excel.

### 📊 Organização estruturada

As informações foram divididas em diferentes abas de acordo com sua finalidade.

Isso evita concentrar todos os dados em uma única tabela.

---

### 🧮 Fórmulas

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

### 📋 Base de dados auxiliar

A aba `BANCOS` funciona como uma tabela auxiliar contendo instituições financeiras.

Esse conceito é importante porque permite separar:

```text
DADOS PRINCIPAIS
        ↓
INFORMAÇÕES DO CONTRIBUINTE

DADOS AUXILIARES
        ↓
LISTA DE INSTITUIÇÕES
```

---

### 📎 Organização de comprovantes

A seção de informes possui campos destinados à identificação dos arquivos utilizados como comprovantes.

Exemplo:

```text
AXEXO 🖇
BANCOX.PDF
```

A ideia é facilitar a associação entre o dado registrado na planilha e seu respectivo documento de origem.

---

# 🧠 Conceitos Aplicados

Embora seja um projeto desenvolvido em Excel, ele envolve conceitos importantes que também aparecem em sistemas de informação e desenvolvimento de software.

### 1. Organização de dados

As informações são separadas de acordo com sua finalidade.

### 2. Estruturação

Cada grupo de informações possui uma seção específica.

### 3. Automação

Os cálculos são realizados automaticamente por fórmulas.

### 4. Padronização

A lista de instituições financeiras evita a necessidade de digitar repetidamente os nomes dos bancos.

### 5. Integridade das informações

A organização dos campos facilita a conferência dos dados antes de utilizá-los.

### 6. Rastreabilidade

A referência aos comprovantes ajuda a relacionar uma informação registrada com seu documento de origem.

---

# 🔄 Fluxo de utilização

O funcionamento pode ser representado da seguinte maneira:

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

| Tecnologia           | Utilização                  |
| -------------------- | --------------------------- |
| Microsoft Excel      | Desenvolvimento da planilha |
| Fórmulas Excel       | Automatização dos cálculos  |
| Tabelas estruturadas | Organização das informações |
| Listas auxiliares    | Padronização dos bancos     |
| Documentos PDF       | Referência aos comprovantes |

---

# 📁 Estrutura do Projeto no GitHub

Uma sugestão de organização do repositório:

```text
imposto-de-renda/
│
├── README.md
│
├── 📊 Imposto de Renda.xlsx
│
├── 📁 documentos/
│   └── comprovantes/
│
└── 📁 imagens/
    └── preview-planilha.png
```

> ⚠️ **Importante:** não publique no GitHub dados reais como CPF, endereço, telefone, e-mail, informações bancárias ou documentos pessoais.

Para um repositório público, utilize **dados fictícios ou anonimizados**, como foi feito no exemplo da planilha.

---

# 🔐 Segurança e Privacidade

Este projeto trabalha com informações potencialmente sensíveis.

Por isso, uma das principais preocupações ao publicar o projeto é a proteção dos dados pessoais.

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

Esse cuidado é especialmente importante porque o GitHub é uma plataforma pública e os arquivos publicados podem ser acessados e copiados por terceiros.

---

# 🚀 Possíveis Evoluções

O projeto pode evoluir de uma simples planilha de organização para uma solução mais completa de controle financeiro.

Algumas possibilidades:

### 📊 Dashboard financeiro

Criar gráficos para visualizar:

* Total por banco;
* Entradas por mês;
* Distribuição das receitas;
* Evolução dos valores;
* Comparativos anuais.

---

### 📅 Controle mensal

Expandir a aba `NOTAS` para registrar todas as entradas do ano.

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

### 🏦 Mais instituições

Permitir o cadastro de mais bancos e instituições financeiras.

---

### 📎 Controle de documentos

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

### 🤖 Automação

Uma evolução futura poderia utilizar:

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

Dessa forma, o projeto poderia deixar de ser apenas uma planilha e evoluir para uma aplicação de organização e análise de dados financeiros.

---

# 📚 O que este projeto demonstra

Este projeto demonstra conhecimentos práticos em:

* Organização de informações;
* Estruturação de dados;
* Excel;
* Fórmulas;
* Automatização de cálculos;
* Modelagem básica de informações;
* Organização financeira;
* Padronização de dados;
* Documentação;
* Segurança e privacidade de dados.

Além disso, demonstra uma habilidade importante para quem está entrando na área de tecnologia:

> **Transformar uma necessidade real em uma solução estruturada.**

---

# 🎓 Aprendizados

Durante o desenvolvimento deste projeto, alguns conceitos importantes podem ser observados:

### Organização é parte da solução

Uma grande quantidade de informações não significa necessariamente que temos uma boa base de dados.

O verdadeiro desafio está em organizar essas informações de forma que sejam:

**fáceis de inserir → fáceis de consultar → fáceis de conferir → fáceis de utilizar.**

### Automação reduz tarefas repetitivas

Uma simples fórmula pode eliminar cálculos manuais e reduzir a possibilidade de erros durante a consolidação dos dados.

### Segurança precisa fazer parte do projeto

Quando trabalhamos com informações financeiras e pessoais, segurança e privacidade não são detalhes adicionais.

Elas fazem parte da própria solução.

---

# ⚠️ Aviso

Este projeto possui finalidade **educacional e de organização de informações**.

A planilha não substitui orientação de contador, profissional tributário ou os sistemas oficiais utilizados para a declaração do Imposto de Renda.

Os dados presentes na versão de demonstração devem ser tratados como **dados fictícios**.

---

# 👨‍💻 Autor

**Cristiano Bonifácio**

Estudante de Tecnologia com foco em:

* 🔐 Segurança da Informação
* 🛡️ Cybersecurity
* ☁️ Cloud Computing
* 🐧 Linux
* 🌐 Infraestrutura de TI
* 🐍 Python
* 💻 Desenvolvimento

---

## ⭐ Projeto

Se este projeto foi útil ou interessante para você, considere deixar uma ⭐ no repositório.

Cada projeto representa uma etapa da construção de um portfólio prático em tecnologia.

---

### 🚀 De uma planilha para uma solução de tecnologia

Este projeto começou com uma necessidade simples:

> **Como organizar informações financeiras de maneira mais estruturada?**

A resposta foi transformar dados dispersos em uma estrutura organizada, documentada e preparada para futuras automações.

E esse é justamente um dos princípios que quero levar para minha jornada na tecnologia:

**identificar problemas, estruturar informações e construir soluções.**
