# Threat Hunting – Execução Suspeita de PowerShell

## Objetivo

Identificar execuções suspeitas de PowerShell que possam indicar atividades maliciosas em endpoints da rede corporativa.

## Hipótese de ameaça

Atacantes frequentemente utilizam PowerShell para executar comandos maliciosos ou scripts em memória.

## Estratégia de busca

Buscar eventos de execução de PowerShell contendo parâmetros suspeitos como:

- encodedCommand
- bypass
- hidden window

## Exemplo de padrão analisado

powershell.exe -encodedCommand

## Etapas da investigação

1. Consulta de logs de execução de processos.
2. Identificação de comandos PowerShell codificados.
3. Verificação do usuário responsável pela execução.
4. Análise da máquina onde ocorreu a execução.

## Técnicas relacionadas (MITRE ATT&CK)

T1059 – Command and Scripting Interpreter

## Resultado

Execução suspeita identificada em um endpoint fora do horário comercial.

## Ações realizadas

- Isolamento do endpoint
- Análise do script executado
- Monitoramento adicional do host
