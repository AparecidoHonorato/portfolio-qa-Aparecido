# Teste Exploratório — Formulário de Cadastro

## Contexto

Durante a análise do formulário de cadastro, o objetivo foi observar como o sistema se comporta diante de diferentes tipos de entrada de dados, simulando o uso real por pessoas com perfis variados. A intenção foi identificar falhas de validação, inconsistências e possíveis riscos para a qualidade das informações armazenadas.

## Ambiente de Teste

* Navegador: Chrome
* Sistema operacional: Windows
* Execução: ambiente local

## Abordagem Utilizada

Foi realizado um teste exploratório, priorizando a interação livre com o formulário e a inserção de dados fora do padrão esperado. Esse tipo de abordagem permite encontrar comportamentos inesperados que muitas vezes não aparecem em testes roteirizados.

O foco principal esteve em:

* qualidade das validações dos campos
* restrições de formato dos dados
* retorno do sistema após o envio

## Principais Observações

### Campo Nome

Foi possível enviar o formulário informando números e caracteres especiais no campo Nome. Esse comportamento pode comprometer a confiabilidade dos dados cadastrados e gerar inconsistências futuras no sistema.

### Campo Senha

O sistema aceita senhas muito curtas, sem exigir um nível mínimo de segurança. Isso pode representar risco para a proteção das contas dos usuários.

### Campo Idade

Foram aceitos valores incoerentes, como números negativos ou fora de uma faixa plausível. A ausência dessa validação pode impactar relatórios, regras de negócio e integridade das informações.

## Conclusão

O formulário apresenta pontos de melhoria importantes relacionados à validação de dados. Ajustes nessas regras podem aumentar a confiabilidade do sistema, melhorar a experiência do usuário e reduzir problemas futuros com dados inconsistentes.

Este teste demonstrou que a exploração livre do sistema é uma estratégia eficiente para identificar falhas que afetam diretamente a qualidade do produto.
