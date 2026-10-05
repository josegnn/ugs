# Fluxo para Solicitação de Recursos OpenShift

## Sumário

- [Objetivo](#objetivo)
- [Princípios Gerais](#principios-gerais)
- [Requisitos para Solicitacao](#requisitos-para-solicitacao)
- [Documentaçao Obrigatoria da Solicitacao](#documentacao-obrigatoria-da-solicitacao)
- [Critérios de Avaliação](#criterios-de-avaliacao)
- [Fluxo Excepcional para Incidentes Criticos](#fluxo-excepcional-para-incidentes-criticos)
- [Concessao Precaria de Recursos](#concessao-precaria-de-recursos)
- [Revisão da Concessão](#revisao-da-concessao)
- [Checklist da Solicitação](#checklist-da-solicitacao)
- [Resultado Esperado](#resultado-esperado)

---

## Objetivo

Estabelecer o procedimento para solicitação de novos recursos computacionais em ambientes OpenShift, garantindo a utilização eficiente da infraestrutura disponível e assegurando que ampliações de capacidade sejam realizadas somente quando efetivamente necessárias para o funcionamento adequado das aplicações.

---

## Principios Gerais

A concessão de recursos computacionais adicionais não deve ser considerada a primeira alternativa para tratamento de incidentes, degradação de desempenho ou problemas operacionais.

Muitas situações podem ser resolvidas por meio de:

- Otimizações de código;
- Ajustes de configuração da aplicação;
- Correção de vazamentos de memória;
- Revisão de consultas a banco de dados;
- Ajustes de concorrência e processamento;
- Correções arquiteturais ou de infraestrutura da própria aplicação.

Dessa forma, solicitações de ampliação de recursos devem ser fundamentadas por evidências técnicas que demonstrem a necessidade do provisionamento solicitado.

---

## Requisitos para Solicitacao

Toda solicitação de ampliação de recursos deverá ser acompanhada de informações que permitam sua adequada avaliação.

Espera-se que a equipe responsável pela aplicação apresente, além do formulário com as informações necessárias preenchido:

> **NOTA:** O formulário pode ser acessado por [este link](https://pfgovbr-my.sharepoint.com/:w:/g/personal/jose_jgnn_pf_gov_br/IQAoq4bQxA1yTaXgXCJsX9vVAaRwaLtjnXJ5feuhfaKDrQs?e=nppE1g). O formulário, após preenchido, deverá ser convertido em PDF e disponibilizado no OneDrive. O link para acesso ao documento, hospedado no OneDrive, deverá constar na descrição do chamado.

### Evidências de Análise Técnica

- Diagnóstico da causa do problema observado;
- Evidências coletadas durante a investigação;
- Métricas e indicadores que demonstrem a limitação enfrentada;
- Impactos observados para usuários ou processos de negócio.

### Ações de Otimização

Sempre que possível, devem ser apresentadas evidências de que ações de otimização já foram realizadas, tais como:

- Correções de código;
- Ajustes de configuração;
- Revisão de processos de execução;
- Melhorias de desempenho identificadas pela equipe técnica.

Caso as otimizações ainda não tenham sido implementadas, deverá ser apresentado plano de ação contendo as atividades previstas e os respectivos prazos.

### Justificativa da Necessidade

A solicitação deverá demonstrar objetivamente:

- Quais recursos estão sendo solicitados;
- O quantitativo pretendido;
- A razão técnica para a ampliação;
- Como os recursos solicitados contribuirão para a solução do problema ou para a operação adequada da aplicação.

---

## Documentacao Obrigatoria da Solicitacao

Toda solicitação de ampliação de recursos deverá ser acompanhada da documentação necessária para subsidiar a análise técnica da demanda.

A ausência das informações mínimas poderá resultar em devolução da solicitação para complementação.

A documentação deverá contemplar, conforme aplicável:

- Identificação da aplicação e do ambiente afetado;
- Descrição detalhada do problema ou da necessidade identificada;
- Evidências técnicas que demonstrem a limitação atual de recursos;
- Métricas de utilização de CPU, memória, armazenamento ou escalabilidade;
- Registro de incidentes relacionados, quando houver;
- Descrição das ações de otimização já executadas;
- Plano de otimização a ser executado, quando aplicável;
- Justificativa técnica para o quantitativo de recursos solicitado;
- Avaliação dos impactos esperados caso os recursos não sejam concedidos;
- Aprovação ou ciência da gestão responsável pela aplicação.

O detalhamento dessas informações deverá ser apresentado por meio do formulário padrão de solicitação de recursos OpenShift.

---

## Criterios de Avaliacao

As solicitações serão analisadas considerando:

- Evidências técnicas apresentadas;
- Consumo atual dos recursos;
- Histórico operacional da aplicação;
- Existência de oportunidades de otimização;
- Disponibilidade de recursos na plataforma;
- Proporcionalidade entre o problema identificado e os recursos solicitados.

A equipe responsável pela plataforma poderá solicitar informações complementares antes da aprovação do pedido.

---

## Fluxo Excepcional para Incidentes Criticos

Em situações emergenciais, especialmente durante incidentes críticos em produção, pode não haver tempo hábil para execução prévia de análises aprofundadas ou otimizações na aplicação.

Nesses casos, a equipe gestora da aplicação poderá solicitar ampliação emergencial de recursos mediante justificativa técnica que demonstre a necessidade imediata da medida para mitigação ou resolução do incidente.

A análise poderá ocorrer em fluxo simplificado, visando restabelecer a normalidade do serviço no menor tempo possível.

### Concessao Precaria de Recursos

Toda ampliação concedida em caráter emergencial será considerada provisória.

Nessas situações:

- Será definido prazo de vigência da concessão;
- O prazo padrão será de até 15 dias, salvo definição diversa da equipe responsável pela plataforma;
- A equipe da aplicação deverá realizar análise técnica detalhada durante o período concedido;
- Deverão ser executadas ações de otimização ou elaborado estudo técnico que demonstre a necessidade permanente dos recursos adicionais.

Durante a vigência da concessão provisória, poderão ser emitidos alertas e notificações à equipe da aplicação informando a proximidade do encerramento do prazo concedido.

### Revisao da Concessao

Ao final do prazo estabelecido, será realizada reavaliação da necessidade dos recursos concedidos.

A manutenção dos recursos dependerá da apresentação de:

- Evidências das otimizações realizadas; ou
- Estudo técnico que demonstre a necessidade permanente da capacidade adicional.

Na ausência dessas informações, os recursos provisionados provisoriamente poderão ser removidos, retornando a aplicação à configuração anterior.

---

## Checklist da Solicitacao

Antes de encaminhar a solicitação, verifique se todos os itens abaixo foram atendidos.

### Informações Gerais

- [ ] Aplicação identificada.
- [ ] Ambiente informado (Desenvolvimento, Homologação ou Produção).
- [ ] Responsável técnico informado.
- [ ] Gestor da aplicação identificado.

### Análise Técnica

- [ ] Problema ou necessidade devidamente descrito.
- [ ] Evidências técnicas anexadas.
- [ ] Métricas de utilização apresentadas.
- [ ] Impactos para o negócio descritos.

### Otimização da Aplicação

- [ ] Foram realizadas ações de otimização e seus resultados foram apresentados.

**OU**

- [ ] Foi apresentado plano de otimização com atividades e cronograma.

### Justificativa do Provisionamento

- [ ] Recursos solicitados detalhados.
- [ ] Quantitativos informados.
- [ ] Justificativa técnica apresentada.
- [ ] Demonstração de que a ampliação solicitada contribuirá para a solução do problema.

### Solicitações Emergenciais

- [ ] Incidente crítico devidamente caracterizado.
- [ ] Necessidade imediata de ampliação justificada.
- [ ] Equipe ciente do caráter temporário da concessão.
- [ ] Equipe ciente da necessidade de posterior estudo ou otimização.

---

## Resultado Esperado

Este processo busca equilibrar dois objetivos fundamentais:

- Garantir agilidade no atendimento de demandas legítimas e incidentes críticos;
- Promover o uso racional dos recursos computacionais da plataforma OpenShift, evitando superdimensionamentos e assegurando a eficiência do ambiente compartilhado.

A ampliação de recursos deve ser entendida como uma decisão técnica baseada em evidências e alinhada às necessidades reais da aplicação e da plataforma.
