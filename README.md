# n8n-ia-agendamento-google-calendar

## Guia dos Arquivos — n8n + WhatsApp + Google Calendar

Este repositório contém os arquivos necessários para rodar um fluxo no n8n que permite realizar agendamentos via WhatsApp, integrando com o Google Calendar de forma automatizada.

### n8n_workflow.json

Arquivo principal do workflow do n8n.
Como usar:

Abra o n8n → cole o conteúdo do JSON.

Esse fluxo já vem configurado para receber mensagens no WhatsApp e criar eventos no Google Calendar.

Ajuste as credenciais da API do Google e do provedor WhatsApp antes de rodar.

### prompt_system_message_agent_1.md

Prompt usado como mensagem de sistema para o Agente 1.
Define regras, tom e comportamento que o agente deve seguir ao interagir.
Como usar:

Copie o conteúdo para dentro do nó do agente no n8n.

Esse arquivo deve ser colado exatamente no campo de system message.

### prompt_system_message_agent_2.md

Prompt de mensagem de sistema para o Agente 2.
Normalmente usado para complementar o fluxo ou dar instruções adicionais ao agente secundário.
Como usar:

Cole esse conteúdo no segundo agente configurado no workflow.
Garante consistência na forma como o agente processa e responde.

### prompt_user_message_agent_2.md

Prompt de mensagem de usuário que direciona a entrada do Agente 2.
Serve como modelo para estruturar a mensagem recebida do WhatsApp antes do processamento.
Como usar:

Utilize esse texto no campo de user message do segundo agente.
Ajuda a manter a interpretação das mensagens mais clara e previsível.
