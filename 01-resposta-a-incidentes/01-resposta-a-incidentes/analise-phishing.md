# Análise de E-mail de Phishing

## Cenário

Usuários reportaram um e-mail suspeito solicitando redefinição de senha através de um link externo.

## Etapas da análise

1. Análise do cabeçalho do e-mail.
2. Verificação do domínio do remetente.
3. Análise da URL presente na mensagem.
4. Comparação com bases de inteligência de ameaças.

## Indicadores de Comprometimento (IOC)

- Domínio suspeito
- URL maliciosa
- Endereço de remetente falsificado

## Ações realizadas

- Bloqueio do domínio no gateway de e-mail
- Remoção das mensagens das caixas dos usuários
- Comunicação aos usuários sobre tentativa de phishing
