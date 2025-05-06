# analise-arquivos-clienes
Análise de arquivos PDF para consolidar dados de clientes em uma tabela e mesclar documentos relacionados. Inclui extração de texto, normalização de nomes, decodificação de status e automação de tarefas. Gera relatórios organizados e PDFs unificados para clientes, com foco em consistência e eficiência.

Descrição do Projeto:

Este projeto tem como objetivo analisar e processar arquivos PDF relacionados a clientes, organizados em uma pasta no Windows. Existem dois tipos principais de documentos:

Planilhas de Comissão:
Contêm informações sobre o status do processo, o nome do cliente e o corretor responsável.
O título dos arquivos segue o padrão: Planilha Comissão nome_do_cliente (Status,Corretor).
Prestações de Contas:
Contêm informações no corpo do documento, como o número do processo e o nome do cliente.
O título dos arquivos segue o padrão: Prestação de Contas nome_do_cliente.

Problemas Identificados
Variações nos nomes dos clientes entre os arquivos (ex.: diferenças de digitação ou formato).
Arquivos de Planilhas de Comissão que não possuem correspondência em Prestações de Contas e vice-versa.
Clientes em situação de espólio, identificados por palavras-chave como "espólio", "espólio de", etc.
Abreviações no status do processo que precisam ser decodificadas (ex.: AC = Acordo, INCT = Incontroverso).

Objetivos do Projeto:
1.Criar uma tabela consolidada contendo:
Nome do cliente.
Número do processo (extraído do corpo das Prestações de Contas).
Status do processo (extraído do título das Planilhas de Comissão).
Nome do corretor (extraído do título das Planilhas de Comissão).

2.Gerar uma pasta com arquivos PDF combinados para cada cliente, unindo informações das Planilhas de Comissão e Prestações de Contas correspondentes.
