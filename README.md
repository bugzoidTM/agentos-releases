# AgentOS para Windows

Sua equipe de agentes de IA rodando neste computador: o ATLAS coordena, os
chefes de divisão distribuem e os especialistas entregam. Conversa por agente,
aprovação humana do que é sensível, agendamentos e memória — tudo local.

## Baixar

**[Baixar a versão mais recente](https://github.com/bugzoidTM/agentos-releases/releases/latest)**
— arquivo `AgentOS-Setup-<versão>.exe`.

## Instalar

1. Rode o `.exe`. Ele instala só para o seu usuário (não pede administrador)
   e cria o atalho "AgentOS".
2. Se o Windows mostrar "O Windows protegeu o computador", clique em
   **Mais informações → Executar assim mesmo** (o instalador ainda não tem
   certificado de assinatura de código).
3. Para os agentes pensarem, instale o [Ollama](https://ollama.com) e rode:

   ```
   ollama pull qwen2.5:3b
   ollama pull qwen2.5:0.5b
   ```

   A conversa com o ATLAS avisa se falta algum modelo.

## Atualizações

O AgentOS se atualiza sozinho: ao abrir e a cada 4 horas ele procura versão
nova aqui, baixa em segundo plano e avisa. A versão nova entra quando o app
reinicia — ou na hora, clicando no aviso ou em "Reiniciar e atualizar" no
ícone da bandeja.

## Onde ficam seus dados

`%APPDATA%\AgentOS` — banco, workspaces e registros. Desinstalar o app não
apaga essa pasta. A chave do cofre e o acesso ao painel ficam cifrados pelo
próprio Windows.

---

Este repositório guarda só os instaladores. O código-fonte é privado (NUTEF).
