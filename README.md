# Painel de Validação OSE

Site estático para publicar no GitHub Pages. Permite anexar arquivos Excel (`.xlsx`, `.xls`) ou CSV no navegador e visualizar tabela, filtros e gráficos.

## Funcionalidades
- Filtros por **Mês Produção**, **Status AS**, **Prefixo** e busca por **SAP**.
- Tela **Tabela de dados** com todas as colunas da planilha.
- Tela **Gráficos**:
  1. Contagem distinta de SAP por Status AS.
  2. Soma de Valor AS por Prefixo.
  3. Contagem distinta de SAP por Prefixo.
- Resumo de registros, SAP distintos e soma de Valor AS.

## Como publicar no GitHub Pages
1. Crie um repositório no GitHub (por exemplo, `painel-validacao-ose`).
2. Envie o arquivo `index.html` para a raiz do repositório.
3. Acesse **Settings → Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**.
5. Escolha a branch `main` e a pasta `/ (root)` e salve.
6. Aguarde a publicação e abra a URL apresentada pelo GitHub Pages.

## Como usar
Abra o site publicado e clique em **Anexar planilha Excel**. Selecione o arquivo para carregar os dados. O arquivo é processado no navegador; não é enviado para um servidor por este código.

## Observações
- A planilha precisa ter cabeçalhos na primeira linha. Os nomes esperados para os cálculos são `SAP`, `Status AS`, `Prefixo`, `Valor AS` e `Mês Produção` (maiúsculas/minúsculas não importam).
- O site lê a primeira aba do arquivo Excel.
- As bibliotecas SheetJS e Chart.js são carregadas por CDN, portanto é necessária conexão com a internet para carregar e exibir planilhas/gráficos.
