# Ficha de Avaliação de Processo (PDD) — Questão 5

> MOLDE. Copie para `entregas/SEU_RA/` e preencha. Escolha **um** cenário (A ou B).

**Cenário escolhido:** <A ou B>

1. **Nome do processo e descrição resumida:**

Nome: Organização e Renomeação Automatizada de Comprovantes em PDF.

Descrição: Processo diário de varredura em uma pasta de rede para capturar novos comprovantes em PDF, extrair a data e o número do documento presentes no nome original do arquivo através de regras fixas, renomeá-los segundo o padrão oficial da empresa e arquivá-los nas pastas de destino correspondentes.

2. **Volume / frequência estimados:**
   
Cerca de 80 a 120 arquivos diários. A execução ocorre em lote, uma vez por dia (rotina agendada).

3. **As entradas são estruturadas?** (sim/não + justificativa)

Sim. As entradas consistem em arquivos digitais em PDF cujos nomes contêm informações textuais padronizadas (data e número), permitindo a extração automatizada de strings por código ou ferramentas de automação sem necessidade de interpretação visual complexa.

4. **As regras são claras e determinísticas?** (sim/não + justificativa)
   
Sim. As regras de manipulação são estritamente lógicas: leitura do nome atual, aplicação de padrão de corte de texto (ex: expressões regulares / regex), remontagem com o novo padrão corporativo ([Data]_[Documento].pdf) e movimentação baseada na árvore de diretórios. Não há margem para subjetividade ou decisão humana.

5. **Veredito — o processo é elegível a RPA?** (justifique com base em regras
   claras, dados estruturados e repetibilidade)
   
Sim, o processo é altamente elegível. Trata-se de uma tarefa repetitiva, maçante e de alto volume que consome tempo da equipe operacional. Por possuir dados estruturados em texto, regras 100% determinísticas e padrão fixo de execução, a automação elimina erros humanos de digitação/organização e garante total conformidade no arquivamento.