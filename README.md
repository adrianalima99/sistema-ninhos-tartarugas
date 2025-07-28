# 🐢 Sistema de Monitoramento de Ninhos de Quelônios
## Tarefa Individual V – Guardião das Tartaruguinhas

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Sistema desenvolvido para apoiar o monitoramento comunitário de ninhos de quelônios em regiões ribeirinhas da Amazônia. Inspirado em projetos como o **Pé-de-Pincha**, integra tecnologia acessível com saberes locais para fortalecer a conservação da biodiversidade.

---

## 🎯 Funcionalidades Implementadas

### ✅ **Requisitos Obrigatórios**
- 📊 **Estrutura de Dados**: Lista com dicionários contendo todos os campos obrigatórios
- 📝 **Cadastro de Ninhos**: Função para adicionar novos registros com validações
- 📈 **5 Estatísticas Obrigatórias**: Total de ninhos, média por risco, ninhos prestes a eclodir, região com mais risco, danificados com predadores
- 🎮 **Menu Interativo**: Interface contínua até o usuário escolher sair
- ✅ **Validações**: Dados numéricos positivos, status permitidos, emojis corretos

### 🚀 **Funcionalidades Extras Implementadas**

#### 💾 **Persistência de Dados**
- **Salvamento Automático**: Dados são mantidos em arquivo JSON (`ninhos_salvos.json`)
- **Carregamento Inteligente**: Sistema carrega dados salvos ou cria lista inicial
- **Backup de Exemplo**: 10 registros de exemplo se não houver dados

#### 📊 **Análises Avançadas**
- **Estatísticas Detalhadas**: Distribuição por status, porcentagens, contagens específicas
- **Relatório Completo**: Visualização detalhada de todos os ninhos
- **Exportação CSV**: Geração de relatório em formato CSV para análise externa

#### 🎯 **Melhorias na Interface**
- **Conversão Automática**: Aceita texto para risco e converte para emoji
- **Formato Brasileiro**: Data/hora no padrão DD/MM/YYYY HH:MM
- **Emojis Informativos**: Exibe risco com emoji + texto explicativo
- **Submenu de Estatísticas**: Opções simples e avançadas

#### 🔍 **Validações Robustas**
- **Tipos de Dados**: Verificação de int, string, bool
- **Ranges Válidos**: Números não negativos
- **Status Permitidos**: Apenas valores aceitos
- **Tratamento de Erros**: Mensagens claras para o usuário

---

## 🏗️ Estrutura de Dados

Cada ninho é representado como um dicionário com:

| Campo | Tipo | Descrição | Exemplo |
|-------|------|-----------|---------|
| `regiao` | string | Nome da área de praia | "Praia Norte" |
| `quantidade_ovos` | int | Número de ovos identificados | 102 |
| `status` | string | Estado do ninho | "intacto", "ameaçado", "danificado" |
| `risco` | string | Nível de risco (emoji) | "🟢", "🟡", "🔴" |
| `dias_para_eclosao` | int | Dias restantes para eclosão | 12 |
| `predadores` | bool | Presença de predadores | True/False |
| `data_hora` | string | Data/hora do cadastro | "15/01/2024 10:30" |

---

## 🚀 Instalação e Uso

### 📋 Pré-requisitos
- Python 3.8+
- Jupyter Notebook

### 🔧 Instalação
1. Clone o repositório
2. Abra o arquivo `tarefa5_i2a2.ipynb` no Jupyter
3. Execute as células em ordem

### 🎮 Como Usar
1. **Execute as células em ordem**
2. **Use o menu interativo** para todas as operações
3. **Para o campo risco**, use:
   - 🟢 **estável**
   - 🟡 **sob observação** 
   - 🔴 **crítico**

---

## 📊 Exemplos de Saída

### 📋 Relatório Completo
```
🐣 Ninho 1
📍 Região:            Praia Norte
🥚 Ovos:              102
🔧 Status:            intacto
🚨 Risco:             🟢 (estável)
⏳ Dias para eclosão: 12
👀 Predadores:        Não
📅 Data/Hora:         15/01/2024 10:30
```

### 📈 Estatísticas
```
🐢 Total de ninhos registrados:      10
🥚 Média de ovos nos ninhos 🔴 (crítico): 89.67
⏳ Ninhos com 5 dias ou menos para eclodir: 3
📍 Região com mais ninhos sob risco: Praia Norte
⚠️ Ninhos danificados com predadores: 3
```

---

## 🛠️ Tecnologias Utilizadas

- **Python**: Linguagem principal
- **JSON**: Persistência de dados
- **CSV**: Exportação de relatórios
- **datetime**: Registro de data/hora
- **Jupyter Notebook**: Ambiente de desenvolvimento

---

## 📚 Conhecimentos Aplicados

### 🐍 Python Básico
- Estruturas de dados (listas, dicionários)
- Controle de fluxo (condicionais, loops)
- Funções e modularização
- Manipulação de arquivos (JSON, CSV)
- Validação de entrada e tratamento de erros

### 🧠 Lógica de Programação
- Organização de código em funções reutilizáveis
- Persistência de dados entre execuções
- Interface interativa e navegação intuitiva
- Documentação com comentários explicativos

---

## 🌱 Impacto Ambiental

Este sistema representa a **união entre tecnologia e conservação**:

- **🐢 Proteção Direta**: Acompanhamento de ninhos em tempo real
- **👥 Empoderamento Comunitário**: Ferramenta acessível para comunidades locais
- **📈 Escalabilidade**: Modelo replicável para outras regiões
- **🎓 Educação Ambiental**: Integração de jovens em projetos de conservação

---


**🌿 Este sistema é mais que uma tarefa técnica - é um elo entre a tradição da conservação oral e a nova geração de inteligência ambiental comunitária.** 