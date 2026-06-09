# 🚀 Projeto de Testes de Software: Garantia de Qualidade no Aplicativo Urban Routes

[![QA Badge](https://img.shields.io/badge/Role-QA%20Analyst-blue.svg)](https://github.com)
[![Testing](https://img.shields.io/badge/Type-Functional%20%26%20UI%20Testing-green.svg)](https://github.com)
[![Status](https://img.shields.io/badge/Status-Completed-success.svg)](https://github.com)

## 🔍 1. Visão Geral do Projeto
Este repositório contém a documentação, planejamento e execução do ciclo de testes para a interface cartográfica e o sistema de rotas do aplicativo web **Urban Routes**. Como Analista de QA responsável pelo projeto, conduzi uma bateria de testes funcionais e de interface para assegurar que a experiência de navegação do usuário e a plotagem de mapas respeitassem os critérios de aceitação e as especificações de design estabelecidas.

---

## 🛠️ 2. Escopo dos Testes
O plano de testes cobriu cenários críticos de ponta a ponta na aplicação:
* **Mecanismos de Busca:** Validação dos campos de entrada de texto "De" e "Para", incluindo sugestões automáticas e comportamento de placeholders.
* **Navegação Cartográfica:** Comportamento de comandos de zoom, mudança de camadas (Mapa vs. Satélite) e transições visuais.
* **Renderização de Elementos:** Validação de renderização 3D, ícones de transporte (metrô), parques e pontos de referência turística.
* **Componentes de UI:** Responsividade de botões de limpeza (botão de cruz) e links institucionais (logotipo).

---

## 📊 3. Resumo Executivo (Métricas de QA)
Os resultados quantitativos obtidos após a execução completa da suíte de testes são apresentados abaixo:

* **Total de Casos de Teste Executados:** 24 cenários
* **Casos Aprovados:** 16 cenários
* **Casos Reprovados:** 8 cenários
* **Bugs Reportados:** 8 defeitos documentados
* **Taxa de Sucesso (Pass Rate):** ~ 66.6%

---

## 🐛 4. Destaques dos Relatórios de Bug (Defeitos Encontrados)
Abaixo estão detalhados alguns dos bugs de maior impacto técnico e de negócio identificados durante o ciclo de regressão:

### 🚨 Falhas Críticas de Negócio (Bloqueantes)
* **BUG-2 & BUG-3 | Falha Crítica na Plotagem Visual de Localizações**
  * **Prioridade:** Alta
  * **Descrição:** Ao inserir e confirmar um endereço válido nos campos de partida ("De") ou destino ("Para"), o mapa permanece estático e não renderiza os respectivos pins de localização.
  * **Impacto:** Bloqueia a principal jornada de valor do produto, impedindo o usuário de visualizar a rota solicitada.

* **BUG-1 | Ausência de Lista de Sugestões Auto-complete**
  * **Prioridade:** Média
  * **Descrição:** A interface falha ao não exibir a lista suspensa com sugestões de endereços ao digitar palavras-chave (ex: "Subway") no destino.

### 🎨 Falhas de Interface e Usabilidade (UI/UX)
* **BUG-4 | Inoperância da Exibição de Estruturas em Relevo 3D**
  * **Prioridade:** Baixa
  * **Descrição:** Ao aplicar zoom máximo sobre grandes objetos cartográficos (como o Aeroporto LAX), os edifícios permanecem planos (2D), divergindo do comportamento tridimensional esperado pelo design.
* **BUG-9 | Logotipo Principal Inoperante ao Clique**
  * **Prioridade:** Baixa
  * **Descrição:** O logotipo do aplicativo altera o cursor do mouse para o modo interativo ("mãozinha"), mas nenhuma ação ou janela informativa é aberta após o clique do usuário.

---

## 💡 5. Competências Técnicas Demonstradas
* **Análise Crítica de Requisitos:** Confronto direto entre os resultados reais obtidos em tela e os critérios de aceitação refinados.
* **Estratégia de Contorno (Workarounds):** Proatividade para contornar bloqueios no sistema (ex: buscar parques manualmente no mapa devido à quebra do motor de busca de texto) para garantir a continuidade e a cobertura dos testes de regressão.
* **Documentação Técnica Padronizada:** Reporte preciso de bugs utilizando terminologia de mercado (Passos para Reprodução, Resultados Esperados e Reais, Severidade e Prioridade).

---

## 📂 6. Artefatos e Evidências
* 📊 **Planilha de Testes Completa:** Os casos de teste detalhados e a matriz de rastreabilidade de defeitos podem ser consultados diretamente na [Planilha de Casos de Teste do Urban Routes](https://docs.google.com/spreadsheets/d/1dG0VjihFrGDI9GfkdUBkFFIacfiGN5Rj/edit?usp=sharing).
* 📸 **Evidências Visuais:** As mídias e capturas de tela utilizadas como evidências para os relatórios de bug encontram-se organizadas na pasta `/evidencias/print1.png` deste repositório.

---
Análise conduzida por Paula R. R. Bizarro.
