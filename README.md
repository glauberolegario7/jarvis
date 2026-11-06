# JARVIS — Assistente Pessoal

Assistente pessoal que funciona como uma secretária virtual: você conversa com ele em português e ele cuida da sua **agenda**, dos **lembretes** e do **controle de gastos**.

**Acesse:** https://glauberolegario7.github.io/jarvis/

## O que ele faz

- **Conversa natural:** "gastei 45 no mercado", "dentista sexta às 15h, me avisa 1 hora antes", "recebi 4.500 de salário", "quanto gastei esse mês?"
- **Foto de comprovante:** mande a foto de um cupom, recibo, Pix ou boleto. Ele lê o valor e registra o gasto, ou cria um lembrete para pagar o boleto.
- **Agenda:** compromissos por dia, com aviso antes do horário.
- **Finanças:** gastos, entradas, saldo do mês, gastos por categoria e orçamento mensal.
- **Instalável:** no celular, abra o site e use "Adicionar à tela inicial".

## Configuração (gratuita)

1. Entre em https://aistudio.google.com/apikey com sua conta Google e clique em **Create API key**. É grátis e não pede cartão.
2. No app, toque na engrenagem (⚙), escolha **Google Gemini — gratuito** e cole a chave.

O plano gratuito do Gemini tem limite de uso por minuto e por dia (mais que suficiente para uso pessoal), e o Google pode usar as mensagens enviadas no plano gratuito para melhorar os modelos dele.
Se preferir, dá para usar o **Anthropic Claude** (pago por uso) com uma chave de https://console.anthropic.com/settings/keys.

A chave e todos os seus dados ficam **somente no seu navegador** (localStorage). Nada é salvo neste repositório. Use **Exportar backup** nas configurações para guardar uma cópia ou levar os dados para outro aparelho.

## Limitações desta versão

- Os dados não sincronizam sozinhos entre aparelhos (use exportar/importar).
- Os lembretes aparecem enquanto o app está aberto (ou em segundo plano recente no navegador).

## Arquivos

- `index.html`: o app inteiro (HTML, CSS e JavaScript)
- `sw.js`: service worker (abrir offline e notificações)
- `manifest.json`: dados para instalar como app
