# [Avançado] Envio Automático de Relatórios por E-mail
Este programa realiza o envio automático de e-mail para os endereços constantes na planilha Gerentes.xlsx.

## Contextualização
Imagine que você seja responsável pela área de inteligência de negócios de uma empresa e que você receba um relatório das seguintes áreas:

- Financeiro
- Logística
- Manutenção
- Marketing
- Operações
- Produção
- Vendas

Cada um desses relatórios — um arquivo .xlsx — deve ser enviado por e-mail para o gerente da respectiva área. O arquivo Gerentes.xlsx contém as informações de contato de cada um deles: nome, e-mail e área.

Para resolver esse problema, foi necessário importar as seguintes bibliotecas:

- os
- dotenv
- pandas
- yagmail

A bilioteca __dotenv__ foi usada para podermos salvar os dados de autenticação da conta de e-mail (nome de usuário e senha) nas variáveis de ambiente do sistema operacional. Por sua vez, a biblioteca
__os__ foi usada para podermos recuperar os valores das variáveis de ambiente NOME_USUARIO e SENHA e autenticar nosso usuário.

Usamos o pandas para poder ler o arquivo Gerentes.xlsx e extrair as informações para compor o e-mail.

## Como Testar
Para testar este código, você deverá criar um arquivo .env e definir seus próprios valores para as variáveis de ambiente NOME_USUARIO e SENHA. Por exemplo:

NOME_USUARIO=teste@gmail.com

SENHA=minha_senha


