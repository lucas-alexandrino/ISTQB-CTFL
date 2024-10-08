# Certified Tester Foundation Level (CTFL) v4.0 [NEW!]

Este repositório contém conteudos e resumos, focados em testes e QA, que aprendi durante o estudo para a certificação CTFL 4.0 e outras certificações do [ISTQB](https://www.istqb.org/).

O conteúdo está ***numerado*** de acordo com os topicos abordados no Syllabus desta versão do CTFL

O exame tem os seguintes domínios do conteúdo e ponderações:

| Capítulos | Questões | Percentagem |
| - | - | ------ |
| 1 | 8 | 26.67% |
| 2 | 6 | 20.00% |
| 3 | 4 | 13.33% |
| 4 | 11| 36.67% |
| 5 | 9 | 30.00% |
| 6 | 2 | 6.67% |
|  | 40 |  |

**Capítulo 1:** Fundamentos dos Testes

**Capítulo 2:** Testes ao longo do ciclo de vida de desenvolvimento de software

**Capítulo 3:** Teste Estático

**Capítulo 4:** Análise e Projeto de Teste

**Capítulo 5:** Gerenciando as atividades de teste

**Capítulo 6:** Ferramentas de Teste

Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request com melhorias ou correções.

## 1.1 O que é Teste?

Conjunto de atividades para:

- Descobrir defeitos
- Avaliar a qualidade dos artefatos de software

> *Artefatos de software* = De acordo com ISTQB, Objetos de teste ou software alvo de teste (o produto de trabalho a ser testado)

> *Objetos de teste:* Amplo

> *Itens de teste:* As funções dos objetos de teste, por exemplo: Site de banco(Objeto de teste) a função de ver saldo (Item de teste).

## Verificação x Validação

![Verificação_Validação](images/verificacao-validacao.png)

***Verificação:***
”Estamos construindo o produto corretamente?”
• O software deve estar de acordo com sua especificação, os requisitos especificados na estória

***Validação:***
”Estamos construindo o produto certo?”
• O software deve fazer o que o usuário realmente deseja

De nada adianta um software que segue todos os requisitos especificados nas estórias do usuário, se o mesmo no dia-a-dia operacional da empresa não atende as necessidades dos usuários.

> Ex: Um software que cumpre todos os requisitos especificados, mas é lento demais para certas tarefas do dia-a-dia.

## Testes estáticos x Testes dinâmicos

![Captura de tela 2024-08-07 114859.png](images/testes_estatico_dinamico.png)

Teste de (Unidade, Unitário e Componente) são os mesmos, e na prova também são, de acordo com o glossário.

> A parte mínima de um sistema que pode ser testado isoladamente.

Teste de uma ou mais unidades(componentes) juntas, é um Teste de integração, ou Teste de integração de componentes

## Imagem Resumo

![Resumo-teste-corrigido.png](images/Resumo-teste-corrigido.png)

## 1.1.1 Objetivos do teste

![objetivos-teste](images/objetivos_teste.png)

**Os objetivos típicos do teste são:**

- Avaliar produtos de trabalho, como requisitos, histórias de usuários, projetos e código;
- Detectar falhas e defeitos;
- Garantir a cobertura necessária de um objeto de teste;
- Reduzindo o nível de risco de qualidade de software inadequado;
- Verificar se os requisitos especificados foram atendidos;
- Verificar se um objeto de teste está em conformidade com os requisitos contratuais, legais e
normativos;
- Fornecer informações aos stakeholders para que eles possam tomar decisões informadas;
- Criar confiança na qualidade do objeto de teste;
- Validar se o objeto de teste está completo e funciona conforme o esperado pelos
stakeholders.

### Comentários:

- ***Detectar falhas e defeitos***
    1. Defeito: o que ocorre no processo de desenvolvimento do software ou nas atividades de **Verificação**, que se caso seja um erro na codificação pode tornar-se um Erro.
    2. Falha: o que ocorre quando o software está em produção, nas atividades de **Validação**, quando o software apresenta comportamento e respostas diferentes do esperado, afetando diretamente a experiência do usuário final.
    
- ***Garantir a cobertura necessária de um objeto de teste***
    1. Cobertura de teste: Ela mede o percentual de linhas testadas, ou seja, quantidade de linhas testadas dividido pelo total de linhas de código.


## 1.1.2 Teste e Depuração

### O teste e a depuração são atividades distintas

O teste pode desencadear falhas causadas por defeitos de software(teste dinâmico) ou pode encontrar defeitos diretamente no objeto de teste (teste estático).

Quando o teste dinâmico aciona uma falha, a **Depuração** se preocupa em encontrar as causas dessa falha(defeitos),analisar essas causas e eliminá-las.

### Processo típico de Depuração(debugging)

1. Reproduzir uma falha 
2. Diagnosticar(encontrar a causa principal)
3. Corrigir a causa

**Teste de confirmação:** verificar se as correções resolveram o problema

**Teste de regressão:** verificar se a correção de um problema não ocasionou falhas em outras partes do objeto de teste.

![teste-depuracao](images/teste_depuracao.png)

## 1.2 Por que os testes são necessários?

![necessidade_teste](images/necessidade_teste.png)

## 1.2.1 Contribuições para o sucesso dos testes

## 1.2.2 Testes e Garantia da Qualidade (QA)

### Teste e QA não são a mesma coisa

- **QA (Quality Assurance ou Garantia da Qualidade)**
    1. Um QA tem o papel um pouco mais amplo do que o de um Tester , deve garantir que todo o processo de desenvolvimento de software esteja dentro dos melhores padrões e práticas que levam à melhor qualidade.
- **Tester (Analista de teste)**
    1. O analista de teste tem como maior objetivo a execução de testes para identificar algum problema ou falha no software. Concentrando seus esforços em testes manuais e automatizados, entre outros.

![qa_qc](images/qa_qc.png)
![discurso_qaqc](images/discurso_qaqc.png)

## 1.2.3 Erros, Defeitos, Falhas e Causas raiz

> ***A mesma coisa** porém em momentos diferentes como uma borboleta(lagarta, casulo, borboleta)*
> 

**Erro(equívoco, engano):** Ação humana que produz um resultado incorreto.

**Causa-Raiz:** Uma fonte de um defeito tal que, se ele for removido, a ocorrência do tipo do defeito é reduzida ou removida.

**Defeito(Falta, bug):** Uma imperfeição ou deficiência em um produto de trabalho que não atende aos seus requisitos ou especificações ou prejudica o uso pretendido.

**Falhas(Problema):** Um evento em que um componente ou sistema não atende a seus requisitos dentro dos limites especificados.

![domino](images/domino.png)

![warning](images/warning.png)

Os erros e defeitos não são a única causa de falhas.

As falhas também podem ser causadas por condições ambientais, como quando a radiação ou o campo eletromagnético causam defeitos no firmware.

## 1.3 Princípios de teste

> **São 7 Fundamentos(Princípios) de teste.**
> 

1. ***O teste mostra a presença, não a ausência de defeitos.*** Questão de cobertura de teste: 100% de cobertura de testes é igual a garantia completa da qualidade?
2. ***Testes exaustivos são impossíveis.*** Testar todas as possibilidades de **entradas** é impossível ,exceto em softwares muitos pequenos.
3. ***Testes antecipados economizam tempo e dinheiro.*** Regra 10 de Myers ou Shift-left
4. ***Os defeitos se agrupam.*** Regra 80/20( Princípio de Pareto)
5. ***Os testes se degradam.*** Se eu testar sempre do mesmo jeito, logo menos os testes não serão mais eficazes para encontrar bugs (Paradoxo do pesticida)
6. ***Os testes dependem do contexto.*** Não existe uma única abordagem universalmente
aplicável aos testes. Os testes são feitos de forma diferente em contextos diferentes . 100 horas para teste em uma Aeronave(Navegação, Entretenimento), Análise de risco.
7. ***Falácia da ausência de defeitos.*** Além da verificação, a validação também deve ser realizada.

## 1.4 Atividades de teste, Testware e Papéis no teste

O teste depende do **contexto**, mas, em um nível elevado, há **conjuntos comuns de atividades de teste** sem os quais é menos provável que o teste atinja seus objetivos. Esses conjuntos de atividades de teste formam um **processo de teste.**

Processo de teste:

> O conjunto de atividades inter-relacionadas que inclui planejamento de teste, monitoramento e controle de teste, análise de teste, modelagem de teste, implementação de teste, execução de teste e conclusão de teste.
>


## 1.4.1 Atividades e Tarefas de Teste

Um **processo de teste** geralmente consiste nos principais grupos de atividades descritos abaixo.

![monitoramento_controle](images/monitoramento_controle.png)

![tabela_processo](images/tabela_processo.jpeg)

***Atenção:***

**Monitoramento x Controle:**

Monitoramento: envolve a verificação contínua de todas as atividades de teste e a comparação do progresso real com o plano

Controle: controle do teste envolve a tomada das ações necessárias para atingir os objetivos do teste.(Caso as atividades de teste não estejam atingindo o plano)

**Execução do Teste:**

Execução dos testes e gerenciamento dos defeitos que aparecerem.

**Modelagem x Implementação:**

Os procedimentos de testes, com o cronograma de execução dos testes(ordem) é apenas na **Implementação**.

**Projeto de teste ou Modelagem:** 

A mesma coisa.

## 1.4.2 Processo de teste no contexto

Os **testes não são realizados de forma isolada**. As atividades de teste são parte integrante dos processos de desenvolvimento executados em uma organização. Os testes são financiados pelos stakeholders e seu objetivo final é **ajudar a atender às necessidades de negócio** deles.

![processo_teste](images/processo_teste.png)

## 1.4.3 Testware 

![testware](images/testware.png)

## 1.4.4 Rastreabilidade entre a Base de teste e o Testware

> ***Rastreabilidade:*** Entender quais foram os requisitos geradores, o que inspirou(Base de teste) os testes a serem criados, e o contrário, quais testes foram criados(Testware), e quais resultados foram produzidos a partir desses requisitos/estórias
> 

Além de avaliar a cobertura, uma boa rastreabilidade permite determinar o impacto das mudanças, facilita as auditorias de teste e ajuda a atender os critérios de governança de TI.

A boa rastreabilidade também torna o progresso do teste e os relatórios de conclusão mais
compreensíveis, incluindo o status dos elementos da base de teste. Isso também pode ajudar a
comunicar os aspectos técnicos dos testes aos stakeholders de uma maneira compreensível.

A rastreabilidade auxilia a parte de Monitoramento e controle do processo de teste

A rastreabilidade fornece informações para avaliar a qualidade do produto, a capacidade do
processo e o progresso do projeto em relação aos objetivos de negócio.

![Rastreabilidade Bidirecional](images/rastreabilidade_teste.png)

## 1.4.5 Papéis no Teste

<p float="left">
  <img src="images/papel_gerente.png" width="400" />
  <img src="images/papel_testador.png" width="400" /> 
</p>

## 1.5 Habilidades essenciais e boas práticas em testes

Soft skills até 1.5.2

## 1.5.1 Habilidades genéricas necessárias para testes

## 1.5.2 Abordagem de equipe completa

## 1.5.3 Independência dos testes

<p float="left">
  <img src="images/independencia1.png" width="400" />
  <img src="images/independencia2.png" width="400" /> 
</p>

**Testadores independentes** provavelmente reconhecerão **diferentes tipos de falhas e defeitos** em comparação com os desenvolvedores, devido às suas diferentes formações, perspectivas técnicas e preconceitos.

Há também algumas **desvantagens**. Os Testadores independentes podem ficar **isolados** da equipe de desenvolvimento, o que pode levar à **falta de colaboração**, a **problemas de comunicação** ou a uma **relação adversa** com a equipe de desenvolvimento.
