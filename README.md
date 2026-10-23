# Pipeline de Testes com Jenkins e Cypress

Projeto educacional para praticar integração contínua de testes automatizados, utilizando Jenkins, Jenkinsfile e Cypress.

## Objetivos
- Definir etapas de pipeline como código.
- Automatizar a execução dos testes Cypress.
- Praticar integração entre repositório, agente de execução e ferramenta de CI.

## Tecnologias
- Jenkins
- Jenkinsfile
- Node.js e npm
- Cypress

## Pré-requisitos
- Jenkins instalado e configurado com um agente compatível.
- Node.js e npm disponíveis no agente.
- Projeto e dependências acessíveis pelo pipeline.

## Como executar
1. Configure um job Pipeline no Jenkins apontando para este repositório.
2. Selecione o Jenkinsfile adequado ao sistema operacional do agente (`Jenkinsfile`, `Jenkinsfile-win` ou a cópia disponível).
3. Confira os comandos e caminhos do arquivo escolhido antes de executar.
4. Execute o job e consulte o console output para verificar a instalação e os resultados dos testes.

Os arquivos Jenkinsfile podem representar variantes da atividade; revise-os antes de escolher um deles.

## Estrutura do projeto
```text
ci-cd-teste-jenkins/
├── Jenkinsfile
├── Jenkinsfile-win
├── Jenkinsfile copy
├── cypress/
├── cypress.config.js
├── package.json
└── README.md
```

## Desafios práticos
Configurar o ambiente de execução, escolher o pipeline compatível com o agente e interpretar falhas causadas por dependências, configuração ou testes.

## Boas práticas adotadas
- Pipeline versionado junto ao projeto.
- Execução automatizada dos testes.
- Uso dos logs do Jenkins para diagnóstico.

## 📚 Aprendizados
A atividade permite praticar conceitos de integração contínua, configuração de pipelines como código e execução automatizada de testes Cypress em um ambiente Jenkins.

## Considerações finais
A execução depende da configuração do Jenkins e do agente. Verifique os caminhos e comandos do Jenkinsfile selecionado, pois há variantes no repositório.

---

## 🎓 Formação
Atividade desenvolvida durante a formação profissionalizante em **Quality Assurance (QA) pela EBAC — Escola Britânica de Artes Criativas e Tecnologia**.