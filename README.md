# Pipeline de Testes com Jenkins e Cypress

Projeto educacional para praticar integração contínua de testes automatizados, utilizando Jenkins, Jenkinsfile, Cypress e relatórios Allure.

## Objetivos
- Definir etapas de pipeline como código.
- Automatizar a execução de testes Cypress em três suítes.
- Praticar execução paralela e publicação de relatórios no Jenkins.

## Tecnologias
- Jenkins Pipeline
- Node.js e npm
- Cypress
- Allure

## Pré-requisitos
- Jenkins instalado e configurado com um agente compatível.
- Node.js disponível no agente e a ferramenta global do Jenkins configurada com o nome `nodejs`.
- Google Chrome disponível no agente para as suítes que o exigem.
- Plugin Allure instalado no Jenkins para a etapa de publicação do relatório.
- Acesso ao repositório e permissão para executar o job.

## Como executar
1. Crie um job do tipo **Pipeline** no Jenkins e conecte-o a este repositório.
2. Para agentes Linux/macOS, use `Jenkinsfile`, que utiliza comandos `sh`. Para agentes Windows, confira `Jenkinsfile-win`, que utiliza `bat`.
3. Antes de executar, confirme se os nomes das ferramentas e os plugins exigidos estão configurados no Jenkins.
4. Execute o job e consulte o console output. O pipeline principal executa as suítes `teste-suite-1`, `teste-suite-2` e `teste-suite-3` em paralelo.
5. Quando a publicação Allure estiver configurada, consulte o relatório na página do build.

## Execução local
Com Node.js/npm instalados, na raiz do projeto:

```bash
npm install
npm run teste-suite-1
npm run teste-suite-2
npm run teste-suite-3
```

As suítes e seus caminhos estão definidos no `package.json`. A disponibilidade do Chrome e a configuração do Cypress podem afetar a execução local.

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

O arquivo `Jenkinsfile copy` é uma variante adicional; confira seu conteúdo antes de selecioná-lo no job.

## Desafios práticos
Configurar o agente, executar suítes em paralelo, interpretar falhas e publicar relatórios de execução.

## Boas práticas adotadas
- Pipeline versionado junto ao projeto.
- Separação dos testes em suítes.
- Uso dos logs do Jenkins para diagnóstico.
- Publicação de resultados como apoio à análise de falhas.

## 📚 Aprendizados
A atividade permite praticar CI, pipeline como código, execução paralela de testes Cypress e integração de relatórios Allure.

## Considerações finais
Os pipelines exigem configuração correspondente ao sistema operacional do agente. Ajuste ferramentas, plugins e caminhos conforme o ambiente Jenkins utilizado.

---

## 🎓 Formação
Atividade desenvolvida durante a formação profissionalizante em **Quality Assurance (QA) pela EBAC — Escola Britânica de Artes Criativas e Tecnologia**.
