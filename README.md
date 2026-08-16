# Dashcilia · Painel da Clícia Estética 💆‍♀️

Sistema **simples de verdade** para a Clícia organizar a clínica pelo celular:

- **Agenda** — atendimentos da semana, com nome da cliente, procedimento, hora e valor. Ao concluir um atendimento, o valor pode ir direto pro caixa.
- **Estoque** — produtos com botões de **+ / −** e aviso automático quando está acabando.
- **Caixa** — o que **entrou** e o que **saiu**, com o saldo do mês na hora.
- **Início** — resumo do dia: agenda de hoje, saldo do mês e alertas de estoque.

Tudo em **um único arquivo** (`index.html`), sem instalar nada, sem login, sem internet depois de aberto. Os dados ficam salvos no próprio celular (localStorage).

## Como colocar no ar (GitHub Pages)

1. No GitHub, vá em **Settings → Pages**.
2. Em *Source*, escolha **Deploy from a branch**, selecione a branch principal e a pasta `/ (root)`.
3. Salve. Em ~1 minuto o site fica disponível em `https://<usuario>.github.io/dashcilia/`.

## Como a Clícia usa no celular

1. Abra o link no navegador do celular.
2. Toque em **Compartilhar → Adicionar à Tela de Início** (iPhone) ou **⋮ → Adicionar à tela inicial** (Android).
3. Pronto — vira um ícone como se fosse um aplicativo.

## Cópia de segurança

Os dados ficam no aparelho. No menu **⋯** (canto superior direito) dá pra:

- **Salvar cópia de segurança** — baixa um arquivo com todos os dados;
- **Restaurar cópia salva** — recupera tudo em um celular novo.

Recomende que ela salve uma cópia de vez em quando (ex.: toda sexta).

## Desenvolvimento

Não há build nem dependências. Para testar, basta abrir `index.html` no navegador.
