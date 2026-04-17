# professional-project
Repositório profissional contendo projetos voltado a análises de dados, automação, melhorias de processo e soluções orientadas a negócio. Desenvolvido para demonstrar habilidades técnicas, organização, boas práticas e pensamento analítico.

🏦 Inteligência de Mercado: Campanhas de Aquisição PJ e Crédito 2026

🎯 1. Contexto e Objetivos
Este projeto utiliza o NotebookLM como um motor de análise competitiva para o setor bancário brasileiro, com foco no público Pessoa Jurídica (PJ). O objetivo é processar dados densos (tarifários, manuais de crédito e relatórios de mercado) para fundamentar estratégias de marketing e vendas para produtos de fomento, especificamente Pronampe e Procred.

Objetivos:

Identificar lacunas tarifárias entre bancos tradicionais e digitais.

Sintetizar regras complexas de crédito governamental em argumentos de venda claros.

Criar um repositório de consultas rápidas para objeções de clientes em campanhas B2B.

📚 2. Curadoria de Fontes
As fontes selecionadas garantem a precisão técnica e evitam alucinações da IA por estarem baseadas em documentos oficiais de 2026:

Tabela Geral de Serviços PJ (Itaú): Acesse o PDF aqui

Relatório Semestral "Onde Investir" (XP): Análise de cenário macro e taxas Selic/IPCA.

Manual de Operações Pronampe (FGO/BB): Diretrizes oficiais sobre garantias e carência.

Cartas Mensais Verde Asset: Visão estratégica de gestores sobre riscos de crédito no Brasil.

🛠️ 3. Engenharia de Prompts e "Cicatrizes"
O mercado valoriza o processo. Abaixo, documento a evolução do raciocínio para extrair o melhor da IA:

💡 Pergunta Estratégica Base
"Extraia os custos de manutenção de conta e taxas de antecipação de recebíveis do PDF do Banco X e compare com o Banco Y."

🩹 Cicatrizes (Troubleshooting & Troubleshooting)
Problema: A IA inicialmente misturava taxas de "Cesta de Serviços" de Pessoa Física com Pessoa Jurídica que estavam no mesmo documento.

Ajuste de Prompt: Adicionei uma instrução de contexto negativo: "Ignore seções de 'Varejo PF'. Extraia apenas dados da seção 'Corporate' e 'Business', focando em empresas com faturamento anual de até R$ 4,8 milhões."

Aprendizado: Descobri que pedir para a IA "pensar passo a passo" antes de montar a tabela comparativa reduzia erros de transcrição de valores numéricos complexos.

📖 4. Miniguia de Estudo (Entrega Final)
📄 Resumo Estruturado: O Cenário PJ em 2026
O mercado bancário PJ em 2026 está polarizado: enquanto bancos digitais dominam a experiência de usuário e taxas zero, bancos tradicionais como Bradesco e Itaú detêm a vantagem no crédito assistido (Pronampe/BNDES) devido à capilaridade física e fundos garantidores consolidados. A grande oportunidade de campanha reside na carência de 12 meses dessas linhas frente ao capital de giro caro dos concorrentes.

📙 Glossário de Conceitos Chave
FGO (Fundo Garantidor de Operações): O mecanismo que permite ao banco emprestar sem exigir imóveis ou veículos como garantia real do empresário.

Spread Bancário: A margem de lucro do banco na operação.

CET (Custo Efetivo Total): A métrica real de comparação; inclui taxa nominal, impostos (IOF) e seguros.

🔄 Prompts Reutilizáveis para Revisão
Análise de Concorrente: "Com base nas novas tabelas de tarifas, cite 3 motivos financeiros para um cliente trocar o Banco X por nós."

Copywriting de Campanha: "Gere um roteiro de 30 segundos para vídeo focado em empresários que precisam de crédito, mencionando a carência de 1 ano do Pronampe."

Autor: [GABRIELA BENEDINI]
Estrategista em Direção Técnica e Inteligência de Dados aplicada ao Marketing Financeiro.
