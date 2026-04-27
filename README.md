QA Bug Report — DOE Website
Relatório de teste realizado no site do Diário Oficial do Estado (DOE), identificando falha de acesso em navegador específico.

Cenário de Teste:
Acesso ao site do DOE via navegador
Problema identificado:
Erro de conexão ao acessar o site no Google Chrome (ERR_CONNECTION_TIMED_OUT)

Ambiente:
Navegador: Google Chrome (erro)
Navegador: Microsoft Edge (funcionando)
Sistema operacional: Windows

Passos reproduzidos:
Acesso ao site e aguardo no carregamento

Resultado esperado:
O site deveria abrir normalmente em todos os navegadores suportados

Testes realizados:
Limpeza de cache (sem sucesso)
Desativação de antivírus/firewall (causa do erro)
Teste em navegador alternativo (funcionou)

Análise Final: 
O site utiliza protocolo HTTP (sem HTTPS).
O antivírus bloqueou o acesso por considerar a conexão insegura

Conclusão:
Possível problema de segurança devido à ausência de certificado SSL, impactando o acesso em determinados ambientes.

Evidências: 
Erro no navegador Google Chrome: https://raw.githubusercontent.com/myrellasouza7/qa-bug-reports/refs/heads/main/Captura%20de%20tela%202026-04-27%20123931.png
Funcionando normalmente no navegador Microsoft Edge: https://raw.githubusercontent.com/myrellasouza7/qa-bug-reports/refs/heads/main/Captura%20de%20tela%202026-04-27%20125809.png
Funcionando normalmente no navegador Google Chrome após desativação do antivírus: https://raw.githubusercontent.com/myrellasouza7/qa-bug-reports/refs/heads/main/Captura%20de%20tela%202026-04-27%20130453.png
