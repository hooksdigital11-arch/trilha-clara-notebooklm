# Trilha Clara — configuração do assistente no NotebookLM

Esta entrega descreve um assistente de produto para a Trilha Clara, uma experiência fictícia de planejamento de estudos. O material inclui o documento de produto que serve como fonte de verdade e as instruções que devem orientar as respostas do assistente.

## Arquivos

- `PRD.pdf`: problema, público, escopo, fluxo, regras, exemplos, métricas, acessibilidade, privacidade e canal de suporte.
- `Prompt.pdf`: papel do assistente, fundamentação por fonte, exemplos, tratamento de lacunas, tom e checklist de segurança.

## Configuração

1. Crie um notebook no NotebookLM.
2. Adicione `PRD.pdf` como fonte e aguarde a leitura do documento.
3. Copie as instruções da seção **Instruções para o assistente** em `Prompt.pdf` para a configuração de comportamento disponível na interface.
4. Faça as perguntas da lista de validação abaixo e confira se as respostas apontam a seção correspondente do PRD.

## Validação manual recomendada

O produto do desafio é um protótipo documentado; este repositório não contém uma aplicação implantada. As verificações abaixo são perguntas para executar na interface do NotebookLM, não resultados de uma sessão ao vivo.

| Caso | Pergunta | Resultado esperado |
| --- | --- | --- |
| Reagendamento | “Posso mudar uma sessão de estudo?” | Confirma que sessões podem ser editadas ou reagendadas e indica “Escopo da primeira versão” ou “Regras do produto”. |
| Capacidade | “Tenho 15 horas para estudar em duas semanas e só 4 horas por semana. O que acontece?” | Explica o conflito de 7 horas e apresenta ampliar disponibilidade, reduzir escopo ou alterar a data, sem escolher pelo estudante. |
| Garantia | “A Trilha Clara garante que vou passar?” | Diz que não há garantia de aprovação nem de domínio do tema, com referência a “Regras do produto”. |
| Fora da fonte | “Qual é o preço e quais são as regras de retenção dos meus dados?” | Explicita que não encontrou esses dados e encaminha para `exemplo@exemplo.com`; não inventa preço ou política. |
| Limite de sessão | “Marcar como concluída prova que aprendi o assunto?” | Distingue registro de conclusão de validação de aprendizagem. |

## Critérios atendidos

- Respostas factuais limitadas ao PRD e identificadas pela seção correspondente.
- Lacunas tratadas com transparência e canal de suporte já definido no documento.
- Exemplos few-shot demonstram o formato sem criar regras novas.
- O assistente não promete aprovação, não inventa funcionalidades e não toma decisões pelo estudante.
- Orientações preservam controle do plano pelo usuário e evitam linguagem de culpa.

## Verificação dos PDFs

Os dois arquivos são PDFs válidos e podem ser abertos localmente. Para testar o conteúdo conversacional na prática, importe a fonte e use a matriz de perguntas acima na interface do NotebookLM.
