# 🏠 Repúblicas MOC - Busca de Moradia Estudantil

Um sistema simplificado e inteligente projetado para auxiliar estudantes que vêm de fora de Montes Claros (MOC) a encontrarem moradias (repúblicas e pensionatos) próximas às suas respectivas instituições de ensino. 

Este projeto foi desenvolvido como um MVP (Mínimo Produto Viável) em apenas 3 dias durante o workshop **"Construção de Software Completo com Auxílio de IA"**, na IV Semana de Sistemas de Informação e I Semana de Inteligência Artificial da **Unimontes**.

## 🚀 Link do Projeto
O sistema está publicado e pode ser testado em tempo real através do link:
👉 [https://jhonatabarbosa-dev.github.io/republicas-moc/](https://jhonatabarbosa-dev.github.io/republicas-moc/)

---

## 💡 O Problema & A Solução

**O Problema:** Mudar-se para uma nova cidade para estudar gera um grande impacto, principalmente na hora de encontrar uma moradia bem localizada sem conhecer a geografia da região.

**A Solução:** Um sistema focado na experiência do usuário onde o estudante simplesmente seleciona a faculdade onde vai estudar, e o software se encarrega de filtrar e exibir apenas as opções de moradia que ficam nos bairros mais próximos ou na região central da cidade.

---

## 🛠️ Estratégia de Desenvolvimento & Arquitetura

Para entregar um software funcional no prazo de 3 dias do workshop, adotei estratégias ágeis de desenvolvimento de software:

* **Arquitetura Serverless (Sem Backend Complexo):** Em vez de construir uma infraestrutura pesada de banco de dados e rotas de API, a modelagem de dados foi feita inteiramente utilizando arquivos estáticos estruturados em formato **JSON** (`instituicoes.json` e `republicas.json`).
* **Mapeamento de Dados Real:** Os dados de bairros e endereços foram populados manualmente combinando pesquisas reais e o meu conhecimento local sobre a cidade de Montes Claros.
* **Filtro por Proximidade:** Desenvolvi uma lógica de varredura dinâmica em **JavaScript** que analisa a matriz de bairros permitidos para a instituição selecionada e renderiza os cards correspondentes em tempo real.
* **Aceleração por IA:** Utilizei o **GitHub Copilot** de forma estratégica dentro do ambiente de nuvem do **GitHub Codespaces** como um assistente de produtividade para refatoração e otimização do fluxo de código.

---

## 🔧 Tecnologias Utilizadas

* **HTML5:** Estruturação semântica da aplicação.
* **Tailwind CSS:** Estilização responsiva e interface moderna em modo escuro (*Dark Mode*).
* **JavaScript (ES6+):** Consumo assíncrono de dados (`Fetch API`) e lógica de filtragem.
* **Git & GitHub:** Controle de versão e histórico de commits.
* **GitHub Pages:** Hospedagem e deploy automatizado da aplicação.

---

## 📂 Estrutura do Repositório

```text
├── index.html          # Interface principal e lógica em JavaScript
├── instituicoes.json   # Banco de dados simulado das faculdades e bairros adjacentes
└── republicas.json     # Banco de dados simulado dos imóveis e contatos