# Dashcilia · Painel da Clícia Estética 💆‍♀️

Sistema **simples de verdade** para a Clícia organizar a clínica pelo celular:

- **Agenda** — atendimentos da semana, com nome da cliente, procedimento, hora e valor. Ao concluir um atendimento, o valor pode ir direto pro caixa.
- **Estoque** — produtos com botões de **+ / −** e aviso automático quando está acabando.
- **Caixa** — o que **entrou** e o que **saiu**, com o saldo do mês na hora.
- **Início** — resumo do dia: agenda de hoje, saldo do mês e alertas de estoque.

Tudo em **um único arquivo** (`index.html`), sem instalar nada, sem login, sem internet depois de aberto. Os dados ficam salvos no próprio celular (localStorage).

## Como colocar no ar (Vercel)

O projeto é estático: **não tem build, não tem dependência, não tem variável de ambiente**. É só importar e publicar.

1. Acesse [vercel.com/new](https://vercel.com/new) e conecte a conta do GitHub.
2. Escolha o repositório **dashcilia** e clique em *Import*.
3. Deixe tudo como veio — o `vercel.json` já define o projeto como estático:
   - *Framework Preset*: **Other**
   - *Build Command*: vazio
   - *Output Directory*: raiz do projeto
4. Clique em **Deploy**. Em cerca de 30 segundos o site está no ar.

Depois disso, todo push na branch de produção republica sozinho.

> **Branch de produção:** hoje a branch padrão do repositório é `claude/dashboard-clinica-estetica-r73n6n`, e é dela que a Vercel vai publicar. Se mais tarde você renomear a branch padrão ou passar a usar `main`, ajuste em **Settings → Git → Production Branch** na Vercel.

### Domínio próprio (opcional)

Em **Settings → Domains** dá pra apontar um domínio dela, por exemplo `app.esteticacomclicia.com.br`. A Vercel cuida do certificado HTTPS automaticamente.

### O que o `vercel.json` faz

- Marca o projeto como estático, sem etapa de build.
- Manda o navegador **sempre buscar a versão mais nova** do `index.html`, para que atualizações apareçam na hora para ela (sem precisar limpar cache).
- Adiciona dois cabeçalhos básicos de segurança (`X-Content-Type-Options` e `Referrer-Policy`).

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
